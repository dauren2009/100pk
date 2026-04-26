n = int(input())

for i in range(1, n + 1):
    if (i % 3 == 0 or i % 5 == 0) and not (i % 15 == 0):
        print(i, end=" ")

n = int(input())

digits = str(n)
power = len(digits)

total = 0
for d in digits:
    total += int(d) ** power

print(total == n)

s = input()

result = ""
count = 1

for i in range(1, len(s)):
    if s[i] == s[i - 1]:
        count += 1
    else:
        result += s[i - 1] + str(count)
        count = 1

result += s[-1] + str(count)ыы

print(result)


s = input()

clean = s.replace(" ", "").lower()

print(clean == clean[::-1])

s = input()
k = int(input())

if len(s) == 0:
    print(s)
else:
    k = k % len(s)
    print(s[-k:] + s[:-k])
