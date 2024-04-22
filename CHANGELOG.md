# Changelog

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
