# Combat System Implementation Guide

## Overview
Combat systems for platformer games, including enemy AI, player attack mechanics, and damage management.

## Core Components
1. Player attack system
2. Enemy AI behaviors
3. Health and damage management
4. Visual feedback for combat

## Implementation Steps

### Step 1: Player Attack System
```csharp
public class PlayerCombat : MonoBehaviour {
    public float attackDamage = 10f;
    public float attackRange = 1.5f;
    public LayerMask enemyLayers;
    
    public void PerformAttack() {
        // Detect enemies in attack range
        Collider2D[] hitEnemies = Physics2D.OverlapCircleAll(
            transform.position, 
            attackRange, 
            enemyLayers
        );
        
        // Apply damage to each enemy
        foreach (Collider2D enemy in hitEnemies) {
            EnemyHealth enemyHealth = enemy.GetComponent<EnemyHealth>();
            if (enemyHealth != null) {
                enemyHealth.TakeDamage(attackDamage);
            }
        }
    }
    
    // Visualize attack range in editor
    void OnDrawGizmosSelected() {
        Gizmos.color = Color.red;
        Gizmos.DrawWireSphere(transform.position, attackRange);
    }
}
```
This implements a melee attack system that detects and damages nearby enemies.

### Step 2: Enemy AI Behavior
```csharp
public class EnemyAI : MonoBehaviour {
    public float moveSpeed = 2f;
    public float detectionRange = 5f;
    public Transform player;
    private Rigidbody2D rb;
    private bool isFacingRight = true;
    
    void Update() {
        if (player != null) {
            float distanceToPlayer = Vector2.Distance(transform.position, player.position);
            
            if (distanceToPlayer <= detectionRange) {
                // Move toward player
                Vector2 direction = (player.position - transform.position).normalized;
                rb.velocity = new Vector2(direction.x * moveSpeed, rb.velocity.y);
                
                // Flip sprite based on movement direction
                if ((direction.x > 0 && !isFacingRight) || (direction.x < 0 && isFacingRight)) {
                    Flip();
                }
            } else {
                // Patrol behavior when player is not detected
                Patrol();
            }
        }
    }
    
    void Flip() {
        isFacingRight = !isFacingRight;
        Vector3 scale = transform.localScale;
        scale.x *= -1;
        transform.localScale = scale;
    }
}
```
This creates a basic enemy AI that patrols and chases the player when detected.

## Parameters to Tune
- Attack Range: Distance at which attacks can hit targets (typically 1-2 units)
- Enemy Detection Range: How far enemies can detect the player (typically 3-7 units)
- Damage Values: Amount of health removed per hit (typically 10-50 points)

## Performance Considerations
- Use object pooling for damage indicators and particle effects
- Limit the frequency of physics overlap checks

## Integration Points
The combat system connects with the health system for damage application and with the animation system for attack animations.