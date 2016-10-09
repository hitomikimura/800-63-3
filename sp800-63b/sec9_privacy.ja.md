<a name="sec9"></a>

<!-- ## 9. Privacy Considerations -->
## 9. プライバシーに対する考慮事項

<!-- These privacy considerations provide supplemental guidance for the requirements in section 4. -->
これらのプライバシーに関する考慮事項は、セクション 4 の要件のための補足的なガイダンスを提供する。

<!-- ### 9.1. Privacy Risk Assessment	 -->
### 9.1. プライバシーリスクアセスメント

<!-- Subsections 4.1.6, 4.2.6 and 4.3.6 require the CSP to conduct a privacy risk assessment for records retention. In conducting a privacy risk assessment, CSPs should consider 1) the likelihood that the records retention could create a problem for the subscriber such as invasiveness or unauthorized access to the information; and 2) the impact if a problem did occur. CSPs should be able to reasonably justify any response they take to identified privacy risks, including accepting the risk, mitigating the risk; and sharing the risk. The use of subscriber consent should be considered a form of sharing the risk, and therefore should only be used when a subscriber could reasonably be expected to have the capacity to assess and accept the shared risk. -->
4.1.6、4.2.6、 4.3.6 のサブセクションでは、レコードの保持についてのプライバシーリスクアセスメントを実施するために CSP を必要とする。 プライバシーリスクアセスメントを実施する際、CSPは以下について考える必要がある。 1) レコードの保持がサブスクライバーが侵害される、情報に不正にアクセスされるなどの問題が発生する可能性。 2) 問題が発生した場合の影響。 CSP はリスク受容、リスク軽減、リスク共有など、特定されたプライバシーリスクをとった場合に起こることを合理的に正当化できるべきである。 サブスクライバーの同意を得ることはリスク共有の形と見なされ、サブスクライバーは適切に評価する能力があること、共有されたリスクを受け入れることが期待される。

<!-- ### 9.2. Privacy Controls -->
### 9.2 プライバシーコントロール

<!-- Section 4.4 encourages CSPs to employ appropriately tailored privacy controls. NIST [[SP 800-53]](#sp800-53) provides a set of privacy controls that CSPs should consider implementing when deploying authentication mechanisms. These controls cover notices, redress and other important considerations for successful and trustworthy deployments.  -->
セクション 4.4 は、適切に調整されたプライバシーコントロールを採用する CSP を奨励する。 NIST [[SP 800-53]](#sp800-53) は、CSP が認証メカニズムをデプロイするときに実装を検討するべき一連のプライバシーコントロールを提供する。 これらのコントロールは、成功し、信頼できるデプロイメントのための通知や救済策、その他の重要な考慮事項をカバーする。

<!-- ### 9.3. Use Limitation -->
### 9.3. 使用制限

<!-- Section 4.4 does not permit the CSP to use information about authenticators collected and maintained in the authentication process for any purpose other than authentication or to comply with law or legal process unless the CSP provides clear notice and obtains consent from the subscriber for additional uses. Care should be taken to ensure that use of such information is limited to its original purpose for collection. If use of such information does not fall within uses related to authentication or to comply with law or legal process, the CSP must provide notice and obtain consent from the subscriber. Consult your Senior Agency Official for Privacy (SAOP) if there are questions about whether proposed agency uses fall within the scope of these uses. This notice should follow the same principles as described in effective notice (see Chapter A, section 8.2) and should not be rolled up into a legalistic privacy policy or general terms and conditions. Rather if there are uses outside the bounds of these explicit purposes, the subscriber should be provided with a meaningful way to understand the purpose for additional uses, and the opportunity to accept or decline. The CSP cannot make acceptance by the subscriber of additional uses a condition of providing authentication services.  -->
セクション 4.4 は、CSP が明確な通知を提供し、サブスクライバーからの同意を取得しない限り、CSPが追加の用途において、認証プロセスの中で認証以外の目的のために収集、維持された Authenticator の情報を使用すること、また法律や法的手続きに従うことを許可しない。 このような情報の使用は、本来の収集目的に限定されていることが保証されるよう注意を払うべきである。 このような情報の使用が認証に関連する用途に該当しない、または法律や法的手続きに従うためのものである場合、 CSP は通知を提供し、サブスクライバーから同意を得る必要がある。 提案された使用方法がこれらの用途の範囲内であるかどうかについて質問がある場合は、自身の Senior Agency Official for Privacy (SAOP) に質問する。 通知は、「効果的な通知」 (チャプター A 、セクション 8.2) で前述したものと同じ原則に従う必要がある。また、杓子定規的にプライバシーポリシーや一般的な利用規約にまとめられるべきではない。 むしろ、これらの明示的な目的の範囲外の使用がある場合、サブスクライバーには、追加使用の目的を理解するための有意義な方法と、承諾または辞退ができる機会が提供されなければならない。 CSP は、サブスクライバーが追加の使用条件を受け入れることを、認証サービスを提供する条件にすることはできない。

<!-- ### 9.4. Agency Specific Privacy Compliance  -->
### 9.4. エージェンシーごとに固有のプライバシー遵守

<!-- Section 4.4 covers specific compliance obligations for federal CSPs. It is critical to involve your agency’s SAOP in the earliest stages of digital authentication system development to assess and mitigate privacy risks and as advise the agency on compliance requirements such as whether or not the collection of PII to issue or maintain authenticators triggers the Privacy Act of 1974 or the E-Government Act of 2002 requirement to conduct a Privacy Impact Assessment. For example, with respect to centralized maintenance of biometrics, it is likely that the Privacy Act requirements will be triggered and require coverage by either a new or existing Privacy Act system of records due to the collection and maintenance of attributes/PII necessary for authentication. The SAOP can similarly assist the agency in determining whether a PIA is required.  -->
セクション 4.4 は、連邦政府の CSP に関する特定の遵守義務をカバーする。 プライバシーリスクを評価、軽減し、コンプライアンス要件について助言するように、デジタル認証システム開発の最初期段階にあなたのエージェンシーの SAOP を参画させることが重要である。 (Authenticator を発行または維持する PII コレクションが、プライバシーインパクトアセスメントを実行するために、the Privacy Act of 1974 または the E-Government Act of 2002 requirement をトリガーするかどうかに関わらず) たとえば、バイオメトリクスの集中保守に関して、 Privacy Act requirements がトリガーされ、認証に必要な属性や PII の収集、維持のために、新規または既存の Privacy Act system of records によってカバーされる必要があるかもしれない。 SAOP は、PIA が必要かどうかを判断する 際、 agency と同様に支援することができる。

<!-- These considerations should not be read as a requirement to develop a Privacy Act System of Records Notice or PIA for authentication alone; in many cases it will make the most sense to draft a PIA and SORN that encompasses the entire digital authentication process or include the digital authentication process as part of a larger programmatic PIA that discusses the program or benefit the agency is establishing online access to.  -->
これらの考慮事項は、単独で Privacy Act System of Records Noticeまたは PIA の開発の要件として読まれるべきでない。多くの場合、それは全体のデジタル認証プロセスを包含する PIA と SORN を起案することで最も多くの意味をなす。または、プログラムを議論する、より大きなプログラムに基づいたPIA、もしくは Agency がオンライン・アクセスを行っている利益の一部としてデジタル認証プロセスを含む。

<!-- Due to the many components of digital authentication, it is important for the SAOP to have an awareness and understanding of each individual component so as to advise appropriately on what compliance requirements apply. Moreover, a thorough understanding of the individual components of digital authentication will enable the SAOP to thoroughly assess and mitigate privacy risks either through compliance processes or by other means. -->
デジタル認証の多くのコンポーネントのために、コンプライアンス要件の適用を適切にアドバイスするために個々のコンポーネントの認知と理解を有することは SAOP にとって重要である。 また、デジタル認証の個々 のコンポーネントを徹底的に理解することは、コンプライアンスプロセス またはほかの手段によって、 SAOP が徹底的にプライバシーリスクを評価、軽減することを可能にするだろう。
