hiera-ref
=========

Reference Hiera tree with example projects.

This is a Hiera tree reference that can be cloned by users of Pokey, so it's
not very useful unless you have access to those classes.  The Hiera
configuration used is defined below.

```

---
:hierarchy:
    - %{::fqdn}
    - %{project}/stage/%{stage}
    - %{project}/flavor/%{flavor}
    - %{project}/role/%{role}
    - %{project}/environment/%{environment}
    - %{project}/default
    - %{region}
    - common/stage/%{stage}
    - common/default

```
