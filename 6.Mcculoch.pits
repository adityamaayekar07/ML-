def mcculloch_pitts(inputs, weights, threshold):
    weighted_sum = sum(i * w for i, w in zip(inputs, weights))
    return 1 if weighted_sum >= threshold else 0

# Define gates
AND_GATE = {
    "weights": [1, 1],
    "threshold": 2
}

OR_GATE = {
    "weights": [1, 1],
    "threshold": 1
}

# Test inputs
test_cases = [(0, 0), (0, 1), (1, 0), (1, 1)]

print("AND Gate:")
for x1, x2 in test_cases:
    output = mcculloch_pitts([x1, x2], AND_GATE["weights"], AND_GATE["threshold"])
    print(f"Input: ({x1}, {x2}) -> Output: {output}")

print("\nOR Gate:")
for x1, x2 in test_cases:
    output = mcculloch_pitts([x1, x2], OR_GATE["weights"], OR_GATE["threshold"])
    print(f"Input: ({x1}, {x2}) -> Output: {output}")
