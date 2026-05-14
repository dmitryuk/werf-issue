# Issue relating werf

Steps to reproduce:
1. `werf build --dev`
2. Call `werf build --dev` again - layers cached properly (v)
3. Create new file `touch Example.php`
4. Call `werf build --dev` again - build started without caching (x)
