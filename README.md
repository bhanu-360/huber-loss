# huber-loss
Y = [5, 8, 3]
Y_pred = [5.7, 7.8, 3.4]
delta = 0.5

L1 = delta * (abs(5 - 5.7) - 0.5 * delta)   # 0.225
L2 = 0.5 * (8 - 7.8) ** 2                  # 0.02
L3 = 0.5 * (3 - 3.4) ** 2                  # 0.08

avg_loss = (L1 + L2 + L3) / 3

print("L1:", L1)
print("L2:", L2)
print("L3:", L3)
print("Average Huber Loss:", avg_loss)
