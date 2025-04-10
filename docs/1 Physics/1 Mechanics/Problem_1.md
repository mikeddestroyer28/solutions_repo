# Problem 1


# Ntvyvubi
plt.plot(angles_deg, ranges, marker='o', linestyle='-', color='blue')
plt.title('Projectile Range vs. Launch Angle (Elevated Launch)')
plt.xlabel('Launch Angle (degrees)')
plt.ylabel('Range (meters)')
plt.grid(True)
plt.show()

# Full angle range visualization
theta_vals = np.linspace(0.1, 89.9, 500)  # Avoid 0 and 90 to prevent undefined behavior
theta_rad = np.radians(theta_vals)
range_vals = [range_function(theta) for theta in theta_rad]

plt.figure(figsize=(10, 6))
plt.plot(theta_vals, range_vals, color='green')
plt.title('Full Range vs Angle of Projection')
plt.xlabel('Angle (degrees)')
plt.ylabel('Range (meters)')
plt.grid(True)
plt.show()
![alt text](image.png)
