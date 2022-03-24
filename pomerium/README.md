# Pomerium

Pomerium is an identity-aware proxy that enables secure access to internal applications. Pomerium provides a standardized interface to add access control to applications regardless of whether the application itself has authorization or authentication baked-in. Pomerium gateways both internal and external requests, and can be used in situations where you'd typically reach for a VPN.

Pomerium can be used to:

- provide a single-sign-on gateway to internal applications.
- enforce dynamic access policy based on context, identity, and device state.
- aggregate access logs and telemetry data.
- a VPN alternative.

> This package contains a deployment in _standalone_ mode.

# SYNOPSIS

```
kustomize build instance | kubectl apply -f -
```

> This package can be configured with `kpt cfg` and by modifying `instance/config/pomerium.yml`.

# Description

Identity-aware proxy in standalone mode

# See also

- https://github.com/pomerium/pomerium
