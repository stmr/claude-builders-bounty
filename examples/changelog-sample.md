# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.1.0] - 2026-08-14

### Breaking Changes
- **[schema]** switch user id format from auto-increment integer to uuid v7 (8a3f910)

### Added
- **[auth]** add OAuth2 PKCE provider flow for native CLI clients (c41b8a1)
- **[export]** add CSV and JSON streaming exports for large datasets (e9102b4)
- **[hooks]** add pre-commit git validation hook for conventional commits (d201e74)

### Fixed
- **[api]** handle network timeout gracefully during token refresh (b82e1c0)
- **[pagination]** fix off-by-one truncation when total items equal page limit (7f3a91c)

### Changed
- **[db]** optimize compound index on user sessions for p99 query latency (5d19a82)
- **[logging]** format structured logs to json in production environments (2c918e7)

### Removed
- **[legacy]** remove deprecated v1 REST auth endpoints (a104b93)

### Documentation
- update installation and quickstart guide in README (f482910)
- add comprehensive API parameter reference for export endpoints (9b1837a)

### Maintenance
- bump dependencies to latest patched releases (3e891c2)
- add integration test matrix across Python 3.9-3.13 (1a74d90)
