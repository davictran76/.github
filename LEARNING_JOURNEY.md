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
| :---: | :--- | :--- | :---: | :---: |
| **01** | [Kiến thức cơ bản về Blockchain](https://github.com/Cyfrin/foundry-full-course-cu#course-blockchain-basics) & [Lưu trữ đơn giản](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-1-simple-storage) | Cú pháp, kiểu dữ liệu, Mapping, Struct, Storage layout | [ ] Chờ nộp | [ ] Pending |
| **02** | [Remix Storage Factory](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-2--remix-storage-factory) | Factory pattern, tương tác ABI, Kế thừa & Overrides | [ ] Chờ nộp | [ ] Pending |
| **03** | [Remix Fund Me](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-3-remix-fund-me) | Chainlink Data Feeds, Revert, Payable, CEI pattern | [ ] Chờ nộp | [ ] Pending |
| **04** | [Gợi ý & Hỏi đáp AI](https://github.com/Cyfrin/foundry-full-course-cu#solidity-101-section-4-ai-prompting-asking-questions-and-getting-help) | Kỹ năng debug prompt, tra cứu tài liệu kỹ thuật | [ ] Chờ nộp | [ ] Pending |
| **05** | [Kho lưu trữ đơn giản Foundry](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-1-foundry-simple-storage) | `forge build`, `anvil`, kịch bản deploy, `cast send/call` | [ ] Chờ nộp | [ ] Pending |
| **06** | [Quỹ đầu tư Foundry (Fund Me)](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-2-foundry-fund-me) | Fuzzing cơ bản, Mocking V2, Forked tests, Cheatcodes | [ ] Chờ nộp | [ ] Pending |
| **07** | [HTML/JS Fund Me](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-3-htmljs-fund-me-quick-fullstack--front-end-tutorial) | Kết nối Web3 Provider (Metamask), function selectors | [ ] Chờ nộp | [ ] Pending |
| **08** | [Xổ số hợp đồng thông minh (Raffle)](https://github.com/Cyfrin/foundry-full-course-cu#foundry-fundamentals-section-4-foundry-smart-contract-lottery) | Chainlink VRF, Chainlink Automation, Custom Errors | [ ] Chờ nộp | [ ] Pending |
| **09** | [Foundry ERC20](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-1-foundry-erc20s) | Tiêu chuẩn EIP-20, OpenZeppelin primitives, testing | [ ] Chờ nộp | [ ] Pending |
| **10** | [NFT Foundry (MoodNFT)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-2-foundry-nfts--moodnft) | Chuẩn ERC-721, SVG on-chain, IPFS, mã hóa Base64 | [ ] Chờ nộp | [ ] Pending |
| **11** | [Foundry DeFi (Stablecoin)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-3-foundry-defi--stablecoin-the-pinnacle-project-get-here) | **DỰ ÁN ĐỈNH CAO:** Cơ chế thế chấp, Mint/Burn, Liquidations | [ ] Chờ nộp | [ ] Pending |
| **12** | [Token tái cơ cấu chuỗi chéo (CCIP)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-4-foundry-cross-chain-rebase-token) | Chainlink CCIP, CCT standard, Rebase token logic | [ ] Chờ nộp | [ ] Pending |
| **13** | [Merkle Airdrop & Chữ ký](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-5-foundry-merkle-airdrop-and-signatures) | Merkle Proofs, EIP-712, xác thực chữ ký ECDSA | [ ] Chờ nộp | [ ] Pending |
| **14** | [Nâng cấp Hợp đồng (Upgrades)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-6-foundry-upgrades) | Proxy patterns (UUPS/Transparent), `delegatecall` | [ ] Chờ nộp | [ ] Pending |
| **15** | [Trừu tượng hóa tài khoản (AA)](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-7-foundry-account-abstraction) | EIP-4337, EntryPoint, `PackedUserOperation`, ZKsync AA | [ ] Chờ nộp | [ ] Pending |
| **16** | [DAO & Quản trị](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-8-foundry-dao--governance) | Governance Tokens, Timelock, On-chain Voting | [ ] Chờ nộp | [ ] Pending |
| **17** | [Bảo mật & Kiểm toán Hợp đồng](https://github.com/Cyfrin/foundry-full-course-cu#advanced-foundry-section-9-smart-contract-security--auditing-for-developers) | Phân tích tĩnh Slither, Invariant Testing, Audit review | [ ] Chờ nộp | [ ] Pending |

**Tiến độ hiện tại:** `0 / 17` hoàn thành (`0%`)

```
Tiến độ: ░░░░░░░░░░░░░░░░░░░░  0/17 (0%)
Cần đạt: ████████████████████  15/17 (85%) để mở khóa CadCAD
```

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

> **Trạng thái hiện tại:** `🔒 LOCKED`
>
> Yêu cầu hoàn thành tối thiểu **85%** danh mục kiểm thử và các bài lab DeFi / Bảo mật nâng cao trước khi kích hoạt kịch bản mô phỏng phát thải 5-Token.

| Điều kiện | Yêu cầu | Trạng thái |
| :--- | :--- | :---: |
| Tỷ lệ hoàn thành khoá học | ≥ 85% (≥ 15/17 phần) | [ ] 0/17 |
| Hoàn thành bài lab DeFi Stablecoin (Phần 11) | Bắt buộc | [ ] Chưa |
| Hoàn thành bài lab Bảo mật & Audit (Phần 17) | Bắt buộc | [ ] Chưa |
| File `CERTIFICATES.md` đầy đủ chứng chỉ on-chain | Bắt buộc | [ ] Chưa |

---

*Cập nhật lần cuối: 2025-09-08 — `davictran76` / reset về học từ đầu*
