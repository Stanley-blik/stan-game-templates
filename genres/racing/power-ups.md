# Power-Ups Implementation Guide

## Overview
Power-up systems for racing games that provide temporary advantages to players during races.

## Core Components
1. Power-up collection mechanics
2. Effect application system
3. Duration management
4. Visual indicators

## Implementation Steps

### Step 1: Power-Up Collection
```csharp
public class PowerUp : MonoBehaviour {
    public PowerUpType type;
    public float duration;
    
    void OnTriggerEnter(Collider other) {
        if (other.CompareTag("Player")) {
            PowerUpManager.Instance.ApplyPowerUp(this);
            Destroy(gameObject);
        }
    }
}
```
This handles the collection of power-ups when the player drives through them.

### Step 2: Power-Up Effects Management
```csharp
public class PowerUpManager : MonoBehaviour {
    public static PowerUpManager Instance;
    
    public void ApplyPowerUp(PowerUp powerUp) {
        switch (powerUp.type) {
            case PowerUpType.SpeedBoost:
                ApplySpeedBoost(powerUp.duration);
                break;
            case PowerUpType.Shield:
                ApplyShield(powerUp.duration);
                break;
        }
    }
    
    private void ApplySpeedBoost(float duration) {
        // Increase vehicle speed temporarily
        playerVehicle.maxSpeed *= 1.5f;
        Invoke("ResetSpeed", duration);
    }
}
```
This manages different power-up effects and their durations.

## Parameters to Tune
- Effect Strength: Multiplier values for each power-up type
- Duration: How long each power-up lasts (typically 3-10 seconds)

## Performance Considerations
- Use object pooling for power-up visuals
- Reset effects cleanly to avoid stacking

## Integration Points
The power-up system connects with the vehicle system to modify behavior and with the UI system to display active effects.