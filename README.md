Solana Program Library (Archived)

⚠️ Notice:
This repository has been archived.
All SPL programs and client packages have been migrated into separate repositories under the solana-program organization
.
This repo remains available for historical reference only. Forks are welcome.

📦 Migration Guide

The following programs have been moved to new repositories:

Program	New Repository
Associated Token Account	associated-token-account

Feature Proposal	feature-proposal

Instruction Padding	instruction-padding

Libraries	libraries

Memo	memo

Record	record

Single Pool	single-pool

Slashing	slashing

Stake Pool	stake-pool

Token	token

Token-2022	token-2022

Token Group	token-group

Token Metadata	token-metadata

Token-2022 Transfer Hook	transfer-hook

👉 Governance programs have been moved to Mythic Project Governance
.

For full docs, see the SPL Documentation
.

🚀 Current Deployments

Only a subset of programs are deployed to Solana Mainnet Beta:

Program	Version	Release
token
	3.4.0	release

associated-token-account
	1.1.0	release

token-2022
	1.0.0	release

governance
	3.1.0	release

stake-pool
	1.0.0	release

account-compression
	0.1.3	release

shared-memory
	1.0.0	commit

feature-proposal
	1.0.0	release

name-service
	0.3.0	release

memo
	3.0.0	release

single-pool
	1.0.1	release
🔒 Audits

Some programs have been audited:

Program	Audit Date	Report
token	2022-08-04	Peer Review

associated-token-account	2022-08-04	Peer Review

token-2022	2023-11-03	OtterSec Audit

stake-pool	2023-12-31	Halborn Audit

account-compression	2022-12-05	OtterSec Audit

shared-memory	2021-02-25	Kudelski Audit

single-pool	2024-01-02	Zellic Audit

Other programs are not audited — fork and deploy at your own risk. See SECURITY.md
 for details.

🛠 Development
Setup

Install Solana CLI tools
.

Install latest Rust stable
.

Install libudev (libudev-dev or libudev-devel depending on OS).

Build On-Chain Programs
# Build all on-chain programs
cargo build-sbf

# Build a specific program
cd <program_name>/program
cargo build-sbf

Run Tests
cargo test      # host-based tests
cargo test-sbf  # BPF program tests

Common Issues

Failed to open: ../../deploy/spl_<program-name>.so → update Rust & Cargo.

libssl.so.1.1 missing → install libssl1.1
.

High CPU/memory → run builds with --jobs 1.

📜 Disclaimer

This repository and its code are provided as-is for educational and reference purposes.
Solana Labs makes no guarantees about accuracy, completeness, or compliance.
Use at your own risk and ensure compliance with U.S. export control and sanctions laws.
