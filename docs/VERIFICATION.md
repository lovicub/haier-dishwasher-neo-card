# v1.2.5 publication verification

The release JavaScript is byte-identical to the owner's independently verified working v1.2.5 baseline. No live Home Assistant resources or appliances were modified or called during publication.

SHA256: `0cd297f4ccb75dd7fe5c76e7145261061d0688b4a26d6e68b8f92d55a203abae`

Validation completed with Node 22 syntax checking and isolated headless Chromium:

- 186 control, availability, animation and responsive-layout assertions passed.
- 49 microinteraction checks passed, including hold/release, cancellation, touch scrolling, keyboard, reduced motion and cleanup.
- Temperature fixtures passed, including selection validation and service routing.
- Remaining-time fixtures passed: 16 state representations, no fabricated countdown, no sensor substitution, PL/DE/EN and widths 260/300/330/390.
- Fresh hero and open-door screenshots rendered from the exact released source with fabricated states; network requests blocked and zero service calls.
- Root filename, JSON manifest and manual/HACS resource path mapping checked against the official HACS dashboard documentation. GitHub's Validate workflow reports remote HACS validation separately. No claim of approval for the HACS default directory.

Every prospective public text file and both PNGs were reviewed. No credentials, private endpoints, personal identity, environment paths, logs, backups or HA configuration are included. Public links are confined to this repository and official HACS documentation. PNGs have image chunks only, with no EXIF/text metadata. The generic product entity defaults remain intact.

The card has no imported libraries or external artwork. SVG paths and gradients are embedded in the source; screenshots are derived from that source. The owner authorized publication of their card under MIT. Product/platform trademarks are not licensed by this project.

Limits: tests use simulated HA entities and Chromium touch emulation, not physical Safari or a live appliance. Integration/cloud behavior, actual temperature and remaining-time semantics are not independently established by these tests. The fixture harness and environment files are intentionally excluded from the public package.
