<a name="sec1"></a>

# 1. <a name="purpose"></a> Purpose
[](
This document provides requirements for enrollment and identity proofing of subscribers that wish to gain access to online resources for each Identity Assurance Level (IAL).  The requirements detail the acceptability, validation, and verification of identity evidence that will be presented by an individual to support their claim of identity. This document also details the responsibilities of Credential Service Providers (CSPs) with respect to establishing and maintaining enrollment records, and binding of authenticators (either CSP issued or subscriber-provided) to the enrollment record. 
)
本書は，それぞれの身元保証レベル(IAL)に応じて，オンライン上にあるリソースへのアクセスを必要としている，利用者の登録と身元確認のための要件を提示している．要件は，アイデンティティをサポートするために個々人によって提示される本人確認証明書類によるの正当性，許容性，有効性についてそれぞれ詳細化されている．また，クレデンシャルサービスプロバイダ(CSP)が登録されたレコードを維持すること，ならびに，”認証するために必要な識別子”(CSPが発行したものあるいは申請者から提供されたもの)と登録されたレコードを紐付けることに関しての要件についても詳細を記述している．

<a name="sec2"></a>

# 2. <a name="intro"></a> Introduction
[](
One of the challenges associated with authenticating people is the association of their online activities with a specific physical person. While there are situations where this is not required or is even undesirable (i.e., use cases where anonymity or pseudonymity are required), there are others where it is important to reliably establish the association with a physical person. Examples include obtaining health care and executing financial transactions. There are also situations where the association is required for regulatory reasons (e.g., Know Your Customer requirements in the financial community) or to establish accountability for high-risk actions (e.g., the release of water from a hydroelectric dam).
)
人々を認証するにあたっての課題の１つは，物理的な存在である特定人物と彼らのオンライン上での行動を関連付けることである．これは，必要ではなかったり望ましいくない場合もある一方で（例えば匿名や偽名の利用が必要なケース），物理的な人物との紐付けを確実に確立することが重要である場合もある．例えば，医療関連情報を取得したり，金融関連の取引を行ったりする場合である．その他，規定上の理由から紐付けが必要な場合や（金融界における顧客管理措置(KYC)の対応など），ハイリスクな行動に対する責任の所在を明確にするために必要な場合もある（水力発電ダムからの水の放出など）．

[](
There are also instances where it is desirable for a relying party (RP) to know something about a user executing a transaction, but not know the real human identity of the person.  For example, in order to maintain integrity of the service, it may be desirable to know the home ZIP Code of a user for purposes of census taking or petitioning an elected official but where it is not necessary or desirable to know the underlying identity of the person. Identity assurance levels provide a method for expressing the level of assurance associated with attributes established by the credential service provider during the proofing process.
)
RPにとっては，トランザクションを実行しているユーザについての何かを知ることが望ましい一方，現実世界での人物のアイデンティティは必要でないようなような場合もある．例えば，サービスの質を維持するため，国税調査や公務員からの嘆願でユーザの郵便番号を知る必要が出てきた場合，それぞれのユーザが物理的にどの人物に紐づくかといった情報まで知ることは必要ではないし，望ましくもない．

## 2.1. Expected Outcomes of Identity Proofing

[](
The objective of identity proofing is to:
)
身元確認の目的は以下に記す通り：  
[](
* Resolve a claimed identity to a single, unique identity within the context of the population of users the CSP serves.
* Validate that all evidence that is supplied is valid (correct) and genuine (not counterfeit or misappropriated).
* Validate that the claimed identity exists in the real world.
* Verify that the claimed identity is associated with the real person supplying the identity evidence.
)

* 主張されたアイデンティティを，CSPの利用者中という文脈において，一意に特定すること．
* 提示された全ての証明書類が有効であり（正しく），本物である（偽造や不正流用されていない）ことを検証すること．
* 主張されたアイデンティティは，現実世界に存在する旨を検証すること．
* 主張されたアイデンティティが，提示されたアイデンティティの証明書類によって現実世界の人物との紐付けられている旨を確認すること．

## 2.2. Identity Assurance Levels

[](
Assurance in a subscriber's identity is described using one of three IALs:
)
申請者のアイデンティティの保証レベルは，以下に記す3つのIALのうちの1つを利用する：

[](
---< 以下の内容は、Executive Summaryに記載のものと全く同じ >---

**Identity Assurance Level 1**:
At this level, there is no requirement for an applicant's identity to be proven.  Any attributes provided in conjunction with the authentication process are self-asserted.

**Identity Assurance Level 2**:
At IAL 2, the claimed identity is proven with evidence that supports the real world existence of the claimed identity and identifies and verifies the person to whom the claimed identity belongs.  IAL 2 introduces the need for either remote or in-person identity proofing.  Attributes MAY be asserted by CSPs to RPs in support of pseudonymous identity with verified attributes.

**Identity Assurance Level 3**:
At Identity Assurance Level 3, in-person identity proofing is required. Identifying attributes must be verified by an authorized and trained representative of the CSP. As with IAL 2, attributes MAY be asserted by CSPs to RPs in support of pseudonymous identity with verified attributes. 

----------------------< ここまで >------------------------
)
**身元保証レベル1**
このレベルでは，申請者の身元証明の確認は必須でない．よって，そのアイデンティティの認証プロセス時に提示されるいかなる属性情報も単に申請者自身が主張している内容でしかない．

**身元保証レベル2**
レベル2におけるアイデンティティでは，現実世界で実在すること，そのアイデンティティがどの個人に対応するかの識別，ならびにそれが検証されていることが証明される．レベル2からは，リモートあるいは対面によるの身元確認が必須となる．CSPからRPに渡される属性情報は，CSPにより検証し証明されているものであり(MAY)，匿名化にも対応している．

**身元保証レベル3**
レベル3においては，対面での身元確認が必須である．属性情報の確認は，認定されているCSPによって証明される内容で行わなければならない．レベル2と同様，CSPからRPに渡される属性情報は，CSPにより検証し証明されているものであり(MAY)，匿名化にも対応している．

[](
At IAL 2 and IAL 3, pseudonymity is enabled by CSP limiting the number of attributes sent, or the way they are presented, to the RP. For example, if an RP needs a valid birthdate but no other personal details, the RP should leverage a CSP to request just the birthdate of the subscriber. It is preferred for the RP to ask the CSP for an attribute claim. For example, if an RP needs to know if a claimant is older than 18 they should request a boolean value, not the entire birthdate for them to evaluate age.
)
身元保証レベル2と3では，CSPからRPに送る属性情報の数に制限をかけること，あるいは提供する方法によりで匿名性を確保することもできる．例えば，R正確な誕生日を必要としているけれども他の詳細な個人情報を必要としていない場合，RPはCSPに要求するのは利用者の誕生日だけにとどめるべきである．RPは属性情報のクレームを利用してCSPに必要な情報のみを要求するのが望ましい．例えば，利用者が18歳より年上か否かを知流必要がある場合，RPはbooleanの値として要求するべきであり，年齢を確認するためといって生年月日全てを要求するべきではない．

[](
Since the individual will have undergone an identity proofing process at enrollment and likely associated with one or more authenticators, transactions are not pseudonymous with respect to individual interactions with the CSP.
)
登録時に身元確認のプロセスを経て，1つ以上の”認証するために必要な識別子”と紐付けられた個人は，CSPとの間のトランザクションにおいてのみ，匿名にはならない．

[](
Detailed requirements for each of the IALs is given in [Section 4](#ial-section) and [Section 5](#ipv-section).
)
それぞれの身元保証レベル(IAL)に必要な要件の詳細は，[Section 4](#ial-section) と [Section 5](#ipv-section) を参照のこと．