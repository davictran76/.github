# 📚 Lộ Trình Học Tập & Nghiệm Thu — `davictran76`

> **Học viên:** Trần Đức Nhân (`davictran76`)
> **Tổ chức / Định danh:** `axioledger.axq`
> **Khoá học tham chiếu:** [Cyfrin Updraft — Foundry Full Course](https://github.com/Cyfrin/foundry-full-course-cu)
> **Mục tiêu mở khóa:** `(01-axioledger-core)` — Mô phỏng hệ kinh tế 5-Token (`$AXQ`, `$VPX`, `$SQX`, `$VRQ`, `$KPX`)

---

## 🏛️ Modal 1 — Bảng Điều Phối Mentor (Lead Web3 Auditor)

### Quy trình Pull Request chuẩn hóa

#### 1. Thiết lập nhánh làm việc

> ⚠️ Không commit thẳng vào `main`. Mỗi bài học tạo nhánh riêng.

```bash
git checkout -b lesson/foundry-section-X
```

#### 2. Tiêu chuẩn PR Description

Mỗi PR gửi về repository phải bao gồm:

| Trường | Nội dung yêu cầu |
| :--- | :--- |
| **Module** | Tên phần học theo giáo trình Cyfrin |
| **Mã kiểm thử** | Kết quả `forge test -vvvv` hoặc `forge coverage` |
| **Proof of Execution** | Transaction hash từ Anvil hoặc Testnet Sepolia |

#### 3. Tiêu chí duyệt PR (Definition of Done)

- [ ] Mã nguồn không có cảnh báo nghiêm trọng từ compiler
- [ ] Đã format mã bằng `forge fmt`
- [ ] Khóa riêng tư không bị lộ — bắt buộc dùng Keystore:
  ```bash
  cast wallet import <KEYSTORE_NAME> --interactive
  # hoặc
  npx hardhat vars set PRIVATE_KEY
  ```

---

## 📋 Modal 2 — Bảng Todo & Lộ Trình (`davictran76`)

### Mục tiêu tối thượng

Hoàn thành **100%** các mốc kỹ thuật, đính kèm chứng chỉ vào `CERTIFICATES.md` để đủ điều kiện mở khóa phase mô hình hóa kinh tế **CadCAD (`01-axioledger-core`)**.

---

### Bảng Kiểm Tra Tiến Độ & Nghiệm Thu Chứng Chỉ

| STT | Phần học | Trọng tâm kỹ thuật | Trạng thái PR | Chứng chỉ / Badge |
| :---: | :--- | :--- | :---: | :--- |
| **01** | [Kiến thức cơ bản về Blockchain](https://github.com/Cyfrin/foundry-full-course-cu#course-blockchain-basics) & [Lưu trữ đơn giản](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-1-simple-storage) | Cú pháp, kiểu dữ liệu, Mapping, Struct, Storage layout | ✅ Hoàn thành | [Chứng nhận Phần 1](https://sepolia.etherscan.io/address/0x5c1ddb86F11BB46D3067C702AC554aEaED9ff8f0#code) |
| **02** | [Remix Storage Factory](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-2--remix-storage-factory) | Factory pattern, tương tác ABI, Kế thừa & Overrides | ⏳ Chờ nộp | [Chứng nhận Phần 2](https://sepolia.etherscan.io/address/0x4A62A8901e6113dEF0AEeEC77E531779cd40da73#code) |
| **03** | [Remix Fund Me](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-3-remix-fund-me) | Chainlink Data Feeds, Revert, Payable, CEI pattern | ⏳ Chờ nộp | [Chứng nhận Phần 3](https://sepolia.etherscan.io/address/0x1b30DA2a868704483143A4D46865Ac9585629fd0#code) |
| **04** | [Gợi ý & Hỏi đáp AI](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-4-ai-prompting-asking-questions-and-getting-help) | Kỹ năng debug prompt, tra cứu tài liệu kỹ thuật | ⏳ Chờ nộp | [Chứng nhận Phần 4](https://sepolia.etherscan.io/address/0x4b3a7F293091708dDD6B8748179aeAF80E9c1bA2#code) |
| **05** | [Kho lưu trữ đơn giản Foundry](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-1-foundry-simple-storage) | `forge build`, `anvil`, kịch bản deploy, `cast send/call` | ✅ Hoàn thành | [Chứng nhận Foundry 1](https://sepolia.etherscan.io/address/0x6c4791c3a9E9Bc5449045872Bd1b602d6385E3E1#code) |
| **06** | [Quỹ đầu tư Foundry (Fund Me)](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-2-foundry-fund-me) | Fuzzing cơ bản, Mocking V2, Forked tests, Cheatcodes | ⏳ Chờ nộp | [Chứng nhận Foundry 2](https://sepolia.etherscan.io/address/0xD7D127991c6A89Df752FC3daeC17540aE8B86101#code) |
| **07** | [HTML/JS Fund Me](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-3-htmljs-fund-me-quick-fullstack--front-end-tutorial) | Kết nối Web3 Provider (Metamask), function selectors | ⏳ Chờ nộp | [Chứng nhận Foundry 3](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-3-nfts) |
| **08** | [Xổ số hợp đồng thông minh (Raffle)](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-4-foundry-smart-contract-lottery) | Chainlink VRF, Chainlink Automation, Custom Errors | ⏳ Chờ nộp | [Chứng nhận Foundry 4](https://sepolia.etherscan.io/address/0x33e1fD270599188BB1489a169dF1f0be08b83509#code) |
| **09** | [Foundry ERC20](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-1-foundry-erc20s) | Tiêu chuẩn EIP-20, OpenZeppelin primitives, testing | ⏳ Chờ nộp | [Chứng nhận ERC20](https://sepolia.etherscan.io/address/0xE0aE410a16776BCcb04A8d4B0151Bb3F25035994#code) |
| **10** | [NFT Foundry (MoodNFT)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-2-foundry-nfts--moodnft) | Chuẩn ERC-721, SVG on-chain, IPFS, mã hóa Base64 | ⏳ Chờ nộp | [Chứng nhận NFT](https://sepolia.etherscan.io/address/0x93c7A945af9c453a8c932bf47683B5eB8C2F8792#code) |
| **11** | [Foundry DeFi (Stablecoin)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-3-foundry-defi--stablecoin-the-pinnacle-project-get-here) | **DỰ ÁN ĐỈNH CAO:** Cơ chế thế chấp, Mint/Burn, Liquidations | ⏳ Chờ nộp | [Chứng nhận DeFi](https://sepolia.etherscan.io/address/0xe5760847db2f10A74Fc575B4803df5fe129811C1#code) |
| **12** | [Token tái cơ cấu chuỗi chéo (CCIP)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-4-foundry-cross-chain-rebase-token) | Chainlink CCIP, CCT standard, Rebase token logic | ⏳ Chờ nộp | ⏳ Pending |
| **13** | [Merkle Airdrop & Chữ ký](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-5-foundry-merkle-airdrop-and-signatures) | Merkle Proofs, EIP-712, xác thực chữ ký ECDSA | ⏳ Chờ nộp | ⏳ Pending |
| **14** | [Nâng cấp Hợp đồng (Upgrades)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-6-foundry-upgrades) | Proxy patterns (UUPS/Transparent), `delegatecall` | ⏳ Chờ nộp | [Chứng nhận Upgrades](https://sepolia.etherscan.io/address/0xaFa4150818b7843345A5E54E430Bd0cAE31B5c0C#code) |
| **15** | [Trừu tượng hóa tài khoản (AA)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-7-foundry-account-abstraction) | EIP-4337, EntryPoint, `PackedUserOperation`, ZKsync AA | ⏳ Chờ nộp | ⏳ Pending |
| **16** | [DAO & Quản trị](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-8-foundry-dao--governance) | Governance Tokens, Timelock, On-chain Voting | ⏳ Chờ nộp | [Chứng nhận DAO](https://sepolia.etherscan.io/address/0x46F3fE2C8aC9e9AE4DEDE1a7a29Ab3BdcFa7eaFc#code) |
| **17** | [Bảo mật & Kiểm toán Hợp đồng](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-9-smart-contract-security--auditing-for-developers) | Phân tích tĩnh Slither, Invariant Testing, Audit review | ⏳ Chờ nộp | [Chứng nhận Audit](https://sepolia.etherscan.io/address/0x766a74f8924C7B07df088fDB0F7D7DbaDd330Fb3#code) |

**Tiến độ hiện tại:** `2 / 17` hoàn thành (`≈ 12%`)

---

## 🔁 Kịch Bản Đẩy Bài Tập & Tạo Pull Request

```bash
# 1. Tạo nhánh làm việc độc lập
git checkout -b feature/fund-me-tests

# 2. Format mã nguồn chuẩn
forge fmt

# 3. Chạy toàn bộ test suite
forge test -vvvv

# 4. Commit và đẩy lên remote
git add .
git commit -m "feat(testing): add fund-me unit tests and mock price feeds"
git push -u origin feature/fund-me-tests
```

Sau khi lệnh hoàn tất → truy cập GitHub → mở Pull Request → đính kèm kết quả kiểm thử → yêu cầu review từ mentor.

---

## 🔓 Điều kiện Mở Khóa Phase CadCAD

> **Trạng thái hiện tại:** `🔒 PENDING`
>
> Yêu cầu hoàn thành tối thiểu **85%** danh mục kiểm thử và các bài lab DeFi / Bảo mật nâng cao trước khi kích hoạt kịch bản mô phỏng phát thải 5-Token.

| Điều kiện | Yêu cầu | Trạng thái |
| :--- | :--- | :---: |
| Tỷ lệ hoàn thành khoá học | ≥ 85% (≥ 15/17 phần) | 🔒 2/17 |
| Hoàn thành bài lab DeFi Stablecoin (Phần 11) | Bắt buộc | 🔒 Chưa |
| Hoàn thành bài lab Bảo mật & Audit (Phần 17) | Bắt buộc | 🔒 Chưa |
| File `CERTIFICATES.md` đầy đủ chứng chỉ on-chain | Bắt buộc | 🔒 Chưa |

---

*Cập nhật lần cuối: 2025-09-08 — `davictran76`*
