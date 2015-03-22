# Project Status #

I started out with a minimal (non-configurable) printf that I was using in my own projects, but it lacked many features of the normal library printf.

### Phase 1 - Missing Features ###

The first phase has been to add enough of the standard features to make the function useful in most situations, leaving out only the most (IMHO) obscure ones. This phase is complete.

### Phase 2 - Configuration ###

Having put all those features in I then had to make them optional so that a minimal implementation takes as little memory as possible. This phase is now pretty much complete.

### Phase 3 - Optimisation ###

This will be targeted at the AVR architecture and will involve more fine tuning to reduce the memory usage and execution time.