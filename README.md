# SemidefiniteModels

[![Build Status](https://travis-ci.org/blegat/SemidefiniteModels.jl.svg?branch=master)](https://travis-ci.org/blegat/SemidefiniteModels.jl)
[![Build status](https://ci.appveyor.com/api/projects/status/cxyq8mnav06gkcw9?svg=true)](https://ci.appveyor.com/project/blegat/semidefinitemodels-jl)
[![Coverage Status](https://coveralls.io/repos/blegat/SemidefiniteModels.jl/badge.svg?branch=master&service=github)](https://coveralls.io/github/blegat/SemidefiniteModels.jl?branch=master)
[![codecov.io](http://codecov.io/github/blegat/SemidefiniteModels.jl/coverage.svg?branch=master)](http://codecov.io/github/blegat/SemidefiniteModels.jl?branch=master)

This package extends MathProgBase with `SDModel` representing a semidefinite programming problem in the following form
```
max ⟨C, X⟩            min ⟨b, y⟩
    ⟨A_i, X⟩ = b_i        ∑ A_i y_i ⪰ C
          X  ⪰ 0
```
