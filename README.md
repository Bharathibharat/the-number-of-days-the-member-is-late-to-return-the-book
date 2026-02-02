# the-number-of-days-the-member-is-late-to-return-the-book
d = int(input("Enter Number of days: "))
fine = 0

if d <= 5:
    fine = d * 0.50
    print("Fine:", float(fine))

elif d <= 10:
    fine = (5 * 0.50) + ((d - 5) * 1)
    print("Fine:", float(fine))

elif d <= 30:
    fine = (5 * 0.50) + (5 * 1) + ((d - 10) * 5)
    print("Fine:", float(fine))

else:
    fine = (5 * 0.50) + (5 * 1) + (20 * 5)
    print("Your Membership is cancelled")
    print("Fine amount (Rs):", float(fine))
