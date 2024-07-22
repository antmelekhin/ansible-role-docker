# Changelog

## [1.5.0](https://github.com/antmelekhin/ansible-role-docker/compare/v1.4.1...v1.5.0) (2024-07-22)


### Features

* add `meta/argument_specs.yml` ([#11](https://github.com/antmelekhin/ansible-role-docker/issues/11)) ([e3db76c](https://github.com/antmelekhin/ansible-role-docker/commit/e3db76cb2917f180a2af71bfb3bcf978d1456321))

## [1.4.1](https://github.com/antmelekhin/ansible-role-docker/compare/v1.4.0...v1.4.1) (2024-07-08)


### Fixes

* revert task that removes conflicting packages ([5c06302](https://github.com/antmelekhin/ansible-role-docker/commit/5c063024143eb2c390bcfe76a8742838a780d86a))

## [1.4.0](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.7...v1.4.0) (2024-07-07)


### Features

* add fedora support ([bd766ec](https://github.com/antmelekhin/ansible-role-docker/commit/bd766ec502ca60b7fa3fba6e7f71b5a69d0d82e6))


### Fixes

* revert containerd package ([6a38123](https://github.com/antmelekhin/ansible-role-docker/commit/6a38123dc4a259ab3632fbe79f4c29aaf3e9acb6))


### Styles

* update common role style ([#10](https://github.com/antmelekhin/ansible-role-docker/issues/10)) ([c24e442](https://github.com/antmelekhin/ansible-role-docker/commit/c24e442c49757777f005309cca92b9b6c65ae717))

## [1.3.7](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.6...v1.3.7) (2024-05-13)


### Documentation

* **README:** update variables documentation ([b799aaa](https://github.com/antmelekhin/ansible-role-docker/commit/b799aaaffb002d93bc126400e4b9bbc1c5e0a802))


### Styles

* add newline to end of file ([da16933](https://github.com/antmelekhin/ansible-role-docker/commit/da1693323fee4e4082121722dad523f8a4f0a7d2))
* fix loop var ([9ac44b3](https://github.com/antmelekhin/ansible-role-docker/commit/9ac44b31b41dedeba48d2c861e667f775ed9c3a4))
* rename tasks ([ad3cc67](https://github.com/antmelekhin/ansible-role-docker/commit/ad3cc67799aaa88924c2e0f6dfc5bdaa77ccc95c))

## [1.3.6](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.5...v1.3.6) (2024-04-25)


### Fixes

* fixed task name ([46369e2](https://github.com/antmelekhin/ansible-role-docker/commit/46369e245b0877c39874fa94959ce4873f90f3de))

## [1.3.5](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.4...v1.3.5) (2024-04-25)


### Documentation

* **README:** fixed examples view ([a3a678f](https://github.com/antmelekhin/ansible-role-docker/commit/a3a678f8618604cfb991c680951f55288461f639))


### Fixes

* fixed running a role in `check_mode` ([de59149](https://github.com/antmelekhin/ansible-role-docker/commit/de5914931bea2fe5826773b49cb418cb07e3cde7))

## [1.3.4](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.3...v1.3.4) (2024-04-24)


### Fixes

* **test:** run linters in its own workflow ([#9](https://github.com/antmelekhin/ansible-role-docker/issues/9)) ([7c9e46d](https://github.com/antmelekhin/ansible-role-docker/commit/7c9e46d772fa2fb835eae476cab25affbb78f1b8))

## [1.3.3](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.2...v1.3.3) (2024-04-22)


### Fixes

* add missing fqcn for modules ([e41d4fa](https://github.com/antmelekhin/ansible-role-docker/commit/e41d4fa64b94d89ff292fa24e5d125a3f2d12300))

## [1.3.2](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.1...v1.3.2) (2024-04-20)


### Fixes

* gpgkey value for redhat-based distros ([dedfe39](https://github.com/antmelekhin/ansible-role-docker/commit/dedfe399faa64c10237c1d8ac2d0129e68163d1a))

## [1.3.1](https://github.com/antmelekhin/ansible-role-docker/compare/v1.3.0...v1.3.1) (2024-04-20)


### Code Refactoring

* update variable names, rm conditional expression, quote strings and rm loop for `include_vars` ([#8](https://github.com/antmelekhin/ansible-role-docker/issues/8)) ([7640f97](https://github.com/antmelekhin/ansible-role-docker/commit/7640f97fc3b25851dd89f86135904d32cfdbac87))


### Continuous Integration

* update release rules ([859c958](https://github.com/antmelekhin/ansible-role-docker/commit/859c958ad32976d21c7eff6d6490de1dbfb458c8))
* update workflows ([f4221f3](https://github.com/antmelekhin/ansible-role-docker/commit/f4221f32540cc5145dc44b2305c443a29f14f612))


### Styles

* add `_docker_apt_local_gpgkey` variable ([09d5432](https://github.com/antmelekhin/ansible-role-docker/commit/09d543246545ec64458b8e8e0f897872f7c31f4a))
* minor changes ([e6fa76c](https://github.com/antmelekhin/ansible-role-docker/commit/e6fa76c005f6408665709fbefccaf0a6a0b74bb5))
* rename some tasks, update description, delete `containerd` from package list ([#6](https://github.com/antmelekhin/ansible-role-docker/issues/6)) ([497987e](https://github.com/antmelekhin/ansible-role-docker/commit/497987eb88df30f8c8d2ad32da1c1a8343b30ba8))
* revert empty line after ansible comment ([cb71ee5](https://github.com/antmelekhin/ansible-role-docker/commit/cb71ee5973fc23ed7073eef4360c3e966aab6148))


### Tests

* added hello-world container run test ([#7](https://github.com/antmelekhin/ansible-role-docker/issues/7)) ([5a2047f](https://github.com/antmelekhin/ansible-role-docker/commit/5a2047f34c8a149fcd2d776bd295015273a8b0f0))

## [1.3.0](https://github.com/antmelekhin/ansible-role-docker/compare/v1.2.1...v1.3.0) (2024-02-05)


### Features

* add docker daemon options ([#5](https://github.com/antmelekhin/ansible-role-docker/issues/5)) ([3f3889a](https://github.com/antmelekhin/ansible-role-docker/commit/3f3889a16a30bb1cf4f54ffb0a82d6add3220d96))

## [1.2.1](https://github.com/antmelekhin/ansible-role-docker/compare/v1.2.0...v1.2.1) (2023-12-27)


### Fixes

* add `ansible_managed` comment to redhat repo template ([2a9ca44](https://github.com/antmelekhin/ansible-role-docker/commit/2a9ca4431781c8d29ec27c8427beae0bc94075f6))

## [1.2.0](https://github.com/antmelekhin/ansible-role-docker/compare/v1.1.0...v1.2.0) (2023-12-27)

### Improvements

* update variable names and add other changes ([#4](https://github.com/antmelekhin/ansible-role-docker/issues/4))

## [1.1.0](https://github.com/antmelekhin/ansible-role-docker/compare/v1.0.1...v1.1.0) (2023-11-12)

### Features

* add `docker_version` variable ([#3](https://github.com/antmelekhin/ansible-role-docker/issues/3)) ([dea362f](https://github.com/antmelekhin/ansible-role-docker/commit/dea362f97132a09ac0613eaec598fc08861957e7))

## [1.0.1](https://github.com/antmelekhin/ansible-role-docker/compare/v1.0.0...v1.0.1) (2023-11-12)

### Code Refactoring

* code minor fixes ([#2](https://github.com/antmelekhin/ansible-role-docker/issues/2)) ([40af4fe](https://github.com/antmelekhin/ansible-role-docker/commit/40af4fe4cb23c5bedcdb326af5edb6aeb995c46a))

### Tests

* add tox ([973f7c3](https://github.com/antmelekhin/ansible-role-docker/commit/973f7c3c0dfe0d9752ca0b11f0130ef42b3c40d6))
* fix molecule container name ([6cae788](https://github.com/antmelekhin/ansible-role-docker/commit/6cae7882ac1009f9a3b782f9f245b0c1c139fb16))

## [1.0.0](https://github.com/antmelekhin/ansible-role-docker/compare/...v1.0.0) (2023-08-20)

### Features

* initial commit ([7ff41a2](https://github.com/antmelekhin/ansible-role-docker/commit/7ff41a2d8cbcae3a86b1b22846724188faea41d2))
