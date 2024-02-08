# Kill-Entertainers-
Raj is organizing a surprise party for his friend Arjun and is busy selecting entertainers while also receiving regular updates from his friend, the mountaineer Ishaan, who calls him from the Himalayas.  Ishaan calls Raj every n minutes, meaning he calls at minutes n, 2n, 3n, and so on. 


n, m, z = map(int, input().split())

entertainers_to_be_sent_away = 0

for minute in range(1, z + 1):
    # Check if the current minute is a multiple of both n and m
    if minute % n == 0 and minute % m == 0:
        entertainers_to_be_sent_away += 1

print(entertainers_to_be_sent_away)
