This is a fork of the [python-hl7](http://github.com/johnpaulett/python-hl7)
library created to aid the EHR's Python 3 migration.

python-hl7 0.2.5 is used heavily by our `labs` module. The API changed
significantly between that version and 0.3.0, which introduced Python 3
support.

This fork mirrors a commit from the upstream repo that adds Python 3
compatibility. It was made after version 0.2.5, but before the 0.3.0 release
commit. The API is the same as version 0.2.5.

The reasoning for using this "unreleased" version is that we can accelerate
Python 3 compatibility work for the `labs` module with greater confidence that
it won't cause issues in production than if we upgraded to later releases,
since that would require application logic changes to remain compatible with
this library.

If you're reading this post-Python 3, please investigate the possibility of
updating the EHR to use official releases again.
