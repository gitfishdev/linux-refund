# Data

All data and calculations are WIP. 

More results, along with source code for supporting calculations, will be made available once ready.

## Directory

Paid refunds (each record has a `tx` field indicating the refund transaction):
  - `user-refund-not-claimed-paid.json`: full refund for bidders who did not claim their tokens and have sent all their tokens to the admin address (Note: this list is final)
  - `user-refund-no-sell-paid-Jun3.json`: full refund for bidders and traders who did not sell their tokens and have sent all their tokens to the admin address (Note: this list will be appended with more users sending tokens to the admin address). sent on June 3rd
  - `user-refund-no-sell-paid-Jun9.json`: same as above but it was sent on June 9th
  - `user-refund-no-sell-paid-Jun10.json`: same as above but it was sent on June 10th
  - `user-refund-no-sell-paid-Jun13.json`: same as above but it was sent on June 13th
  - `user-refund-no-sell-paid-Jun14.json`: same as above but it was sent on June 14th
  - `user-refund-linux-recycled-paid-Jun14.json`: full refund for users who had a loss but returned all their $LINUX tokens to the admin address (or sold it). sent on June 14th
  - `user-refund-misc-paid.json`: misc refunds for different edge cases.

Unpaid refunds:
  - `user-refund-linux-not-recycled.json`: refund for users who had a loss but did not return all their $LINUX tokens to the admin address.
