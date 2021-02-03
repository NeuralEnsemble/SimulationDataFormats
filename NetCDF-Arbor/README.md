The Arbor [NSuite](https://github.com/arbor-sim/nsuite) validations use NetCDF
as an internal format for collecting simulation results and for reference data
usef for comparison. They follow a fairly
[minimal set of conventions](https://nsuite.readthedocs.io/en/latest/validation.html#netcdf-conventions),
and are not really intended for use outside the validation suite.

The three files here come from the Arbor rc-expsyn validation test:

* `ref-rc-expsyn-default.nc`

   Reference time series data for the simulation output, computed using scipy.integrate to
   high precision.

* `arbor-rc-expsyn-default-delta.nc`

   The time series output from the Arbor validation run.

* `arbor-rc-expsyn-default-run.nc`

   The difference between the Arbor output data and the interpolated reference data.

Note that the time points in the reference data and the simulation output data are different.
