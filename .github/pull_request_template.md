### PR Security Checklist for UAT/Prod Release:

- [ ] No hardcoded secrets, API keys, or credentials（シークレット/APIキー/認証情報のハードコードなし）
- [ ] Input validation implemented for new/modified endpoints（新規/変更エンドポイントに入力バリデーション実装済）
- [ ] Users can only access their own data — IDOR check（ユーザーは自身のデータのみアクセス可 — IDORチェック済）
- [ ] Error responses do not expose internal details（エラーレスポンスに内部情報を露出していない）
- [ ] PII is not logged or exposed in error messages（PIIがログやエラーメッセージに出力されていない）
- [ ] Items marked N/A have justification noted（N/Aとした項目には理由を記載）

---

### PR Quality Checklist for merging features into develop branch

- [ ] **Impact:** Checked affected modules, dependencies, and backward compatibility with previous app version.
- [ ] **Logic:** Verified implementation against requirements and relevant edge cases.
- [ ] **Financial:** Verified calculation formulas, rates, and rounding (if applicable).
- [ ] **Concurrency:** Checked duplicate execution, race conditions, and idempotency (if applicable).
- [ ] **UI:** Compared UI/text changes with Figma (if applicable).
- [ ] **Integration:** Checked environment configuration and external API error handling via mock service (if applicable).
- [ ] **Cross-platform:** Checked impact on supported platforms and active versions.
- [ ] **Self-test:** Tested the changed functionality and relevant existing flows.
