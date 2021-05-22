# Ansible Collection - jam82.test

Documentation for the collection.

## dependency part of molecule.yml

```yaml
dependency:
  name: galaxy
  options:
    requirements-file: collections.yml
    role-file: requirements.yml
```

## collections.yml

```yaml
---

collections:
  - name: git+https://github.com/jam82/ansible-collection-test.git
    version: main
```

This automatically installs into the namespace defined in `galaxy.yml`.

## usage in role tasks/main.yml

```yaml
    - name: "Collection test"
      jam82.test.my_test:
        name: "Just a test message"
```

cool :)
