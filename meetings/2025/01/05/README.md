# Working Session, 2025-01-05

## Location, Shin Chon Sullungtang and Café V

## Session commenced: 11:30 am

## Activity

* The USDC DIY Charts++s were not working. Debugged this issue. It appears that, since USDC is the ultimate token-data collected, the newline is embedded into
the cell-value, making the coversion from string-to-number fail.
* Prototyped a solution. It didn't work. Debugging revealed s.trim() is a function, but trim as a mapping function doesn't work, because: curse you, o objects!
* Corrected mapping to use object method instead of (non-exant) function trim. That worked.

## Session concluded: 2:30 pm
