# Contributing

Thank you for helping make skill reviews clearer and more useful.

## Good contributions

- A small synthetic example with a well-explained permission or data-flow boundary.
- A counterexample showing why a suspicious-looking instruction can be legitimate in a specific context.
- A correction backed by current primary documentation.
- Clearer language, navigation, accessibility, or a translation that preserves the limitations.

Start with an issue for a large addition. Small documentation fixes can be submitted as a pull request.

## Example format

Use the structure in [examples](examples/README.md): the legitimate user task, a short quoted excerpt, a question for the reader, and expandable review notes. Include evidence locations, unknowns, and a proportionate next step.

Keep examples original, synthetic, and non-executable. Use placeholders instead of real services, customer names, credentials, or targets. Do not add installable `SKILL.md` files, payloads, shell commands, workflows that execute examples, encoded instructions, or hidden Unicode. Describe a hidden instruction visibly instead of actually hiding it.

Clearly label every example as educational material. Do not fabricate scanner output, a numerical score, a real incident, detection accuracy, or endorsement.

## Public contributions are public

Before posting an issue or pull request:

- Remove private code, personal data, internal repository URLs, credentials, and customer information.
- Replace a real scan report with the smallest synthetic example that explains the problem.
- Confirm that you have the right to share the material.
- For a vulnerability in UNPWNED or a report involving sensitive evidence, follow [SECURITY.md](SECURITY.md) instead.

Do not use an issue to request or publish private scanner internals. Do not make accusations about an identifiable project based only on a synthetic exercise or a scanner flag.

## Review checklist for a pull request

- [ ] The contribution is useful without requiring a purchase or signup.
- [ ] The task, requested behavior, unknowns, and reasoning are distinguishable.
- [ ] Examples are synthetic reading material with no executable behavior.
- [ ] No private information, real target, secret, or misleading product claim is included.
- [ ] Relative links work, headings are clear, and images have useful alt text.
- [ ] The original writing can be contributed under the repository's [CC BY 4.0 license](LICENSE).

You retain your rights in your contribution and license the original written material you submit under CC BY 4.0. Contributing to these guides does not require using the hosted service or accepting its separate service terms.

Contributing does not require a star or social promotion. Be constructive, focus on the evidence, and avoid personal attacks or unsolicited promotion. Maintainers may close contributions that do not fit the educational scope.
