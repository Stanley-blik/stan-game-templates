# Movement Systems Implementation Guide

## Overview
Implementation of precise character movement systems for platformer games, including running, jumping, and special movement abilities.

## Core Components
1. Ground detection
2. Jump physics
3. Horizontal movement
4. Special abilities (dash, wall jump, double jump)

## Implementation Steps

### Step 1: Ground Detection
```csharp
public class CharacterMovement : MonoBehaviour {
    public bool isGrounded;
    public float groundCheckDistance = 0.1f;
    public LayerMask groundLayerMask;
    
    void Update() {
        CheckGrounded();
        // Handle movement input...
    }
    
    void CheckGrounded() {
        // Cast a ray downward to check for ground
        RaycastHit2D hit = Physics2D.Raycast(transform.position, Vector2.down, groundCheckDistance, groundLayerMask);
        isGrounded = hit.collider != null;
        
        // Visualize in editor
        Debug.DrawRay(transform.position, Vector2.down * groundCheckDistance, isGrounded ? Color.green : Color.red);
    }
}
```
This implements reliable ground detection using raycasting.

### Step 2: Jump Physics
```csharp
public float jumpForce = 10f;
private Rigidbody2D rb;

void HandleJump() {
    if (isGrounded && Input.GetButtonDown("Jump")) {
        rb.velocity = new Vector2(rb.velocity.x, jumpForce);
    }
    
    // Variable jump height - reduce upward velocity if jump button is released early
    if (rb.velocity.y > 0 && !Input.GetButton("Jump")) {
        rb.velocity = new Vector2(rb.velocity.x, rb.velocity.y * 0.5f);
    }
}
```
This creates responsive jump physics with variable jump height based on input timing.

## Parameters to Tune
- Jump Force: Initial upward velocity (typically 10-15 units)
- Ground Check Distance: How far to check for ground (typically 0.1-0.2 units)
- Gravity Scale: Physics gravity multiplier for character (typically 2-4)

## Performance Considerations
- Cache component references to avoid frequent GetComponent calls
- Use LayerMasks to limit ground detection to relevant objects only

## Integration Points
The movement system connects with the animation system for visual feedback and with the level system for interaction with platforms and obstacles.