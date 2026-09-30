# SafeGate — ETHGlobal ETHOnline 2026 Review Source

SafeGate is a commerce verification and evidence layer.

Payment proves value moved.
SafeGate proves what happened next and makes the strength of that proof explicit.

## Review provenance

This public-review package is reconstructed directly from immutable Git commits associated with the ETHOnline work.

### Hedera x402

Branch:
ethonline-2026-hedera-x402

Pinned commit:
b029028116439c58bfde43becb4889c2be4d2c43

The demonstrated flow was:

Agent
→ HTTP 402
→ Hedera payment verification / settlement
→ request/payment binding
→ single-use consumption
→ paid service execution
→ response hash
→ signed CommerceProof
→ HCS evidence anchor

The replay path rejects reuse of the same payment before executing the service again.

Trust level for the demonstrated result:
OBSERVED

OBSERVED does not mean independently validated.

## The Graph continuity

Branch:
ethonline-2026-thegraph-continuity

Pinned commit:
e141aa2d889dcd64425ea4a9c2d78f79d323f79a

The continuity commit contains the Hedera commit in its ancestry.

The files under thegraph-continuity/ are the files from that pinned continuity commit whose repository paths matched The Graph / Agent0 related work.

## Boundary

SafeGate is not:

- a payment rail
- a wallet
- an escrow service
- a custodian
- a bank
- a marketplace

This directory is a reviewer source package.

It does not expose private production credentials, wallet secrets or private SafeGate Core material.

## Historical integrity

This package does not claim that a hackathon submission form was changed after submission.

It preserves reviewer-accessible source material from the pinned historical commits above.