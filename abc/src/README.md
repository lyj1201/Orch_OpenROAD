# Add new functions
## Operation analysis only without graph updates
```bash
orewrite
oresub
orefactor
```

## Orchestration with specified choice priority
```bash
Ochestration -x rwr -o -y ref -K 8 -z res -O
```
-x, -y, -z is the prioeity order with 'rwrite, ressub, refactor', -o is the zero switch for rewrite, -O is the zero switch for resub, -K is the window setting for refactor.

## Orchestration with random choice
```bash
Ochestration2 -n 10
```
-n is the iteration number for run the random chosen ochstration

