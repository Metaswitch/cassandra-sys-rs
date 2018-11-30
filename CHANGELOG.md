## 0.12.0 (unreleased)
* Upgraded cassandra-cpp-driver to 2.10.0 to get datastax's fix for CPP-499

* Upgraded to version 2.8.0 of the C++ driver (was previously 2.4.3).  See that project's [CHANGELOG](https://github.com/datastax/cpp-driver/blob/master/CHANGELOG.md) for more details.  We noticed the following breaking changes:
  * `cass_error_result_actual` becomes `cass_error_result_responses_received`
  * `cass_error_result_required` becomes `cass_error_result_responses_required`
  * `CASS_WRITE_TYPE_UKNOWN` becomes `CASS_WRITE_TYPE_UNKNOWN`

### 0.11.0 (2017-09-11)

- Regenerate using latest bindgen. Some type incompatibilities are possible, so bumping version as a precaution.

### 0.10.0 (2017-08-02)

- Remove extraneous dependencies (e.g., log).
- Move examples to be proper examples.
- Remove use of error-chain; this is inappropriate for a -sys crate.
- Fix some warnings.
- Correct names of `cass_error_result_received`/`_required`.

### Historical note regarding version 0.9.0

At one point some development was done on preparing a version 0.9.0
using a newer version of bindgen, but the work was not completed or released. See the
[version-0.9](https://github.com/Metaswitch/cassandra-sys-rs/tree/version-0.9) branch
to follow that development. In due course this may be merged to master, but for the moment we recommend you use the
released versions.

### 0.8.8 (2017-06-29)

- Fork crate.
- Remove unused method `cass_cluster_set_queue_size_log`.

### 0.8.7 (2016-12-15)

- (Pre-fork version.)
