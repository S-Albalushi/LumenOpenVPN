# Lumen OpenVPN

Rebranded fork of [ics-openvpn](https://github.com/schwabe/ics-openvpn),
maintained for the Lumen VPN app.

## Why a separate app

Lumen is AGPL-3.0; ics-openvpn is GPL-2.0 with additional terms. The
two licenses do not combine into one binary, but ics-openvpn's license
explicitly permits controlling it from another app over its AIDL API,
so the two apps talk over Binder and neither license bleeds into the
other.

## Changes from upstream

- applicationId: `net.kramb.lumen.openvpn`. The namespace and the
  Java/Kotlin package tree are unchanged, so the internal code matches
  upstream 1:1 and future rebases stay cheap.
- README replaced; original kept as README-upstream.md.

## License

GPL-2.0 with the OpenSSL and Apache-2.0 additional terms, identical to
upstream. See doc/LICENSE.txt.
