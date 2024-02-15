OC-SCORE uses Intel intrinsics. This fork makes use of `simd-everywhere` so OC-SCORE can be compiled for other architectures as well. Tested on Apple Silicon.

To compile this fork, make sure you have the `simd-everywhere` header files and that they are in the include path of your C compiler.

## Specific instructions for Mac

Install `simd-everywhere`:

```
brew install simde
```

Compile OC-SCORE:

```
CPATH="$CPATH:$(brew --prefix)/include" python setup.py build_ext --inplace
```

# OC-SCORE: Detecting Evasion Attacks in Deployed Tree Ensembles

## Installing OC-SCORE

Activate your environment, e.g., using `venv`:
```
python -m venv my_new_venv
source my_new_venv/bin/activate
```

Install dependencies:
```
pip install cython numpy dtai-veritas
```

Compile OC-SCORE:
```
python setup.py build_ext --inplace
```

## Using OC-SCORE

```python
import ocscore

```

## Cite this work

Devos, L., Perini, L., Meert, W., Davis, J. (2023). [Detecting Evasion Attacks in Deployed Tree Ensembles.](https://link.springer.com/chapter/10.1007/978-3-031-43424-2_8) In: Koutra, D., Plant, C., Gomez Rodriguez, M., Baralis, E., Bonchi, F. (eds) Machine Learning and Knowledge Discovery in Databases: Research Track. ECML PKDD 2023. Lecture Notes in Computer Science(), vol 14173. Springer, Cham. https://doi.org/10.1007/978-3-031-43424-2_8
