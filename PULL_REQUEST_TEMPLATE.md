#### PR Security Checklist:

- [ ] No hardcoded secrets, API keys, or credentials（シークレット/APIキー/認証情報のハードコードなし）
- [ ] Input validation implemented for new/modified endpoints（新規/変更エンドポイントに入力バリデーション実装済）
- [ ] Users can only access their own data — IDOR check（ユーザーは自身のデータのみアクセス可 — IDORチェック済）
- [ ] Error responses do not expose internal details（エラーレスポンスに内部情報を露出していない）
- [ ] PII is not logged or exposed in error messages（PIIがログやエラーメッセージに出力されていない）
- [ ] Items marked N/A have justification noted（N/Aとした項目には理由を記載）
