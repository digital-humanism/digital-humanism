<div align="center">
  <a href="https://human-authority.com/">
    <img src="./assets/humanist-banner.png"
         alt="Human authority for controlled AI execution. Human Agency Continuity Protocol."
         width="100%" />
  </a>
</div>

**Capability does not confer authority.**

HUMANIST develops **HACP — Human Agency Continuity Protocol**, a deterministic protocol and enforcement model that keeps protected AI-agent actions within explicit, verifiable human authority before execution.

Authority is evaluated against scoped intent and current control state. The resulting decision is enforced at an explicit boundary, independently of model reasoning.

### Explore the project

| Specification                                                  | SDK / Core                                                             |
| :------------------------------------------------------------- | :--------------------------------------------------------------------- |
| [**hacp-spec**](https://github.com/digital-humanism/hacp-spec) | [**humanist-core**](https://github.com/digital-humanism/humanist-core) |
| Protocol semantics, canonical binding, vectors and conformance | Developer SDK and reference authorization logic                        |

| Enforcement                                                          | Verification                                                                     |
| :------------------------------------------------------------------- | :------------------------------------------------------------------------------- |
| [**hacp-sidecar**](https://github.com/digital-humanism/hacp-sidecar) | [**Conformance & evidence**](https://human-authority.com/standards/conformance/) |
| External fail-closed enforcement and deployment integration          | Conformance families, reproducible results and limitations                       |

### Independent Ada/SPARK Reproduction

[**hacp-sidecar-ada**](https://github.com/digital-humanism/hacp-sidecar-ada) — a technically self-contained Ada/SPARK implementation and public reproduction surface for the HACP 1.1.1 release composition.

The repository provides independent implementation evidence, including canonical conformance, authorization, runtime verification and HTTP workload reproduction.

Its relationship to `hacp-spec`, `hacp-sidecar` and `humanist-core` is documentary and architectural, not a local execution dependency.

This implementation is not currently registered as an additional official `hacp-spec` implementation and does not claim automatic replacement of the existing enforcement sidecar.

**Interactive Reference Surface:** [human-authority.com](https://human-authority.com/) · [Glass House](https://human-authority.com/glass-house/) · [Playground](https://human-authority.com/playground/) · [Documentation](https://human-authority.com/docs/) · [IETF publication](https://human-authority.com/standards/)

### Verification snapshot

Evidence families are reported separately, **not summed into a synthetic overall score**.

| Evidence family                                     | Published result                                                                                                                                                    |
| :-------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| HACP-Core canonical conformance                     | Go 38/38 · TypeScript 38/38 · Python 38/38; Rust 36 direct + 2 adjudicated / 38                                                                                     |
| HC2-55 request binding                              | 55/55 per implementation (Go, TypeScript, Python, Rust)                                                                                                             |
| Anti-bypass deployment evidence                     | 5/5 PASS                                                                                                                                                            |
| Go workload with real upstream forwarding           | 5000/5000 PASS                                                                                                                                                      |
| **Ada/SPARK independent reproduction — HACP 1.1.1** | Core 38/38 · HC2 55/55 · Authorization-v2 3/3 · Runtime 5/5 · HTTP negative PASS · HTTP single valid PASS · HTTP canonical load 100/100 warmup + 5000/5000 measured |

The Ada/SPARK results are reported as a separate reproduction family and do not extend the official implementation-registration claims of `hacp-spec`.

These results have distinct scopes and do not, by themselves, establish deployment security. See the [verification documentation](https://human-authority.com/docs/verification/) for the existing verification families, and the [Ada/SPARK reproduction matrix](https://github.com/digital-humanism/hacp-sidecar-ada/blob/RELEASE/1.1.1/test/matrix/README.md) for the independent reproduction workflow and its boundaries.

### Project origin

The [Digital Humanism Manifesto](https://github.com/digital-humanism/manifesto) establishes the broader human-agency premise. The protocol specification, implementations and interactive reference surface have their own distinct scopes and license terms.
