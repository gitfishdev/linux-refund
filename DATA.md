# Data

All data and calculations are WIP. 

More results, along with source code for supporting calculations, will be made available once ready.

## Directory

Paid refunds (each record has a `tx` field indicating the refund transaction):
  - `user-refund-not-claimed-paid.json`: full refund for bidders who did not claim their tokens and have sent all their tokens to the admin address (Note: this list is final)
  - `user-refund-no-sell-paid.json`: full refund for bidders and traders who did not sell their tokens and have sent all their tokens to the admin address (Note: this list will be appended with more users sending tokens to the admin address)
  - `user-refund-misc-paid.json`: full refund for users who sent funds directly to the program managed accounts.

Unpaid refunds:
  - `user-partial-refund-linux-returned.json`: partial refund for users who had a loss but returned all their $LINUX tokens.
  - `user-partial-refund-linux-not-returned.json`: partial refund for users who had a loss but did not return all their $LINUX tokens.
