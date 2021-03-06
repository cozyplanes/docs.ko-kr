# [WCF 기능 정보](index.md)
## [워크플로 서비스](workflow-services.md)
### [워크플로 서비스 개요](workflow-services-overview.md)
### [장기 실행 워크플로 서비스 만들기](creating-a-long-running-workflow-service.md)
### [메시징 작업](messaging-activities.md)
### [방법: 메시징 작업을 사용하여 워크플로 서비스 만들기](how-to-create-a-workflow-service-with-messaging-activities.md)
### [워크플로에서 계약 사용](using-contracts-in-workflow.md)
### [워크플로 서비스 호스팅 개요](hosting-workflow-services-overview.md)
#### [워크플로 서비스 호스팅](hosting-workflow-services.md)
#### [워크플로 서비스 호스트 내부 기능](workflow-service-host-internals.md)
#### [워크플로 서비스 호스트 확장성](workflow-service-host-extensibility.md)
#### [워크플로 제어 끝점](workflow-control-endpoint.md)
#### [방법: IIS에서 서비스가 아닌 워크플로 호스팅](how-to-host-a-non-service-workflow-in-iis.md)
#### [방법: Windows Server AppFabric을 사용하여 워크플로 서비스 호스팅](how-to-host-a-workflow-service-with-windows-server-app-fabric.md)
#### [WorkflowServiceHost 구성](configuring-workflowservicehost.md)
##### [방법: WorkflowServiceHost를 사용하여 지속성 구성](how-to-configure-persistence-with-workflowservicehost.md)
##### [방법: WorkflowServiceHost를 사용하여 추적 구성](how-to-configure-tracking-with-workflowservicehost.md)
##### [방법: WorkflowServiceHost를 사용하여 유휴 동작 구성](how-to-configure-idle-behavior-with-workflowservicehost.md)
##### [방법: WorkflowServiceHost를 사용하여 워크플로의 처리되지 않은 예외 동작 구성](config-workflow-unhandled-exception-workflowservicehost.md)
### [상관 관계](correlation.md)
#### [상관 관계 개요](correlation-overview.md)
#### [컨텍스트 교환](context-exchange-correlation.md)
#### [영속 이중](durable-duplex-correlation.md)
#### [내용 기반](content-based-correlation.md)
#### [요청-회신](request-reply-correlation.md)
#### [상관 관계 문제 해결](troubleshooting-correlation.md)
### [워크플로 서비스에서 OperationContext 액세스](accessing-operationcontext-from-a-workflow-service.md)
### [워크플로 서비스 내에서 ID 정보 액세스](accessing-identity-information-inside-a-workflow-service.md)
### [워크플로 서비스에서 Serialization 구성](configuring-serialization-in-a-workflow-service.md)
### [방법: 워크플로 응용 프로그램에서 서비스 액세스](how-to-access-a-service-from-a-workflow-application.md)
### [순서에 상관없이 메시지 처리](out-of-order-message-processing.md)
### [트랜잭션을 워크플로 서비스 내부 및 외부로 이동](flowing-transactions-into-and-out-of-workflow-services.md)
### [Send 작업의 캐시 공유 수준 변경](changing-the-cache-sharing-levels-for-send-activities.md)
### [방법: 다른 워크플로 서비스를 호출하는 워크플로 서비스 만들기](how-to-create-a-workflow-service-that-calls-another-workflow-service.md)
### [워크플로 솔루션에 서비스 참조 추가](adding-a-service-reference-in-a-workflow-solution.md)
### [WorkflowServiceHost에서 Side-by-side 버전 관리](side-by-side-versioning-in-workflowservicehost.md)
## [끝점: 주소, 바인딩 및 계약](endpoints-addresses-bindings-and-contracts.md)
### [주소](endpoint-addresses.md)
### [바인딩](bindings.md)
#### [시스템 제공 바인딩 구성](configuring-system-provided-bindings.md)
#### [바인딩에 시간 제한 값 구성](configuring-timeout-values-on-a-binding.md)
#### [UDP 전송을 사용하여 멀티캐스트 응용 프로그램 만들기](creating-multicasting-applications-using-the-udp-transport.md)
### [계약](contracts.md)
#### [ServiceModel 특성 및 ServiceDescription 참조](servicemodel-attributes-and-servicedescription-reference.md)
#### [요청-회신 서비스](request-reply-services.md)
#### [방법: 요청-회신 계약 만들기](how-to-create-a-request-reply-contract.md)
#### [단방향 서비스](one-way-services.md)
#### [방법: 단방향 계약 만들기](how-to-create-a-one-way-contract.md)
#### [이중 서비스](duplex-services.md)
#### [방법: 이중 계약 만들기](how-to-create-a-duplex-contract.md)
#### [방법: 계약 클래스를 사용하여 서비스 만들기](how-to-create-a-wcf-contract-with-a-class.md)
#### [방법: 계약 인터페이스를 사용하여 서비스 만들기](how-to-create-a-service-with-a-contract-interface.md)
#### [ServiceThrottlingBehavior를 사용하여 WCF 서비스 성능 제어](using-servicethrottlingbehavior-to-control-wcf-service-performance.md)
### [방법: 구성에서 서비스 끝점 만들기](how-to-create-a-service-endpoint-in-configuration.md)
### [방법: 코드에서 서비스 끝점 만들기](how-to-create-a-service-endpoint-in-code.md)
### [방법: Svcutil.exe를 사용하여 컴파일된 서비스 코드 유효성 검사](how-to-use-svcutil-exe-to-validate-compiled-service-code.md)
### [표준 끝점](standard-endpoints.md)
## [데이터 전송 및 Serialization](data-transfer-and-serialization.md)
### [서비스 계약에서 데이터 전송 지정](specifying-data-transfer-in-service-contracts.md)
### [데이터 계약 사용](using-data-contracts.md)
#### [방법: 클래스 또는 구조체에 대한 기본 데이터 계약 만들기](how-to-create-a-basic-data-contract-for-a-class-or-structure.md)
#### [직렬화 가능 형식](serializable-types.md)
#### [데이터 계약 이름](data-contract-names.md)
#### [데이터 계약 동등성](data-contract-equivalence.md)
#### [데이터 멤버 순서](data-member-order.md)
#### [데이터 계약 알려진 형식](data-contract-known-types.md)
#### [이후 버전과 호환되는 데이터 계약](forward-compatible-data-contracts.md)
#### [데이터 계약 버전 관리](data-contract-versioning.md)
#### [버전 독립적 Serialization 콜백](version-tolerant-serialization-callbacks.md)
#### [데이터 멤버 기본값](data-member-default-values.md)
#### [상호 운영 가능한 개체 참조](interoperable-object-references.md)
#### [데이터 계약 직렬 변환기에서 지원하는 형식](types-supported-by-the-data-contract-serializer.md)
##### [데이터 계약의 컬렉션 형식](collection-types-in-data-contracts.md)
##### [데이터 계약의 XML 및 ADO.NET 형식](xml-and-ado-net-types-in-data-contracts.md)
##### [데이터 계약의 열거형 형식](enumeration-types-in-data-contracts.md)
### [데이터 계약 직렬 변환기](data-contract-serializer.md)
#### [Serialization 및 Deserialization](serialization-and-deserialization.md)
#### [스키마 가져오기 및 내보내기](schema-import-and-export.md)
##### [스키마를 가져와 클래스 생성](importing-schema-to-generate-classes.md)
##### [클래스에서 스키마 내보내기](exporting-schemas-from-classes.md)
##### [SerializationBinder를 사용하여 serialization 및 deserialization 제어](controlling-serialization-and-deserialization-with-serializationbinder.md)
#### [데이터 계약 확인자 사용](using-a-data-contract-resolver.md)
### [XmlSerializer 클래스 사용](using-the-xmlserializer-class.md)
#### [방법: XmlSerializer를 사용하여 WCF 클라이언트 응용 프로그램의 시작 시간 개선](startup-time-of-wcf-client-applications-using-the-xmlserializer.md)
### [메시지 계약 사용](using-message-contracts.md)
### [서명되거나 암호화된 사용자 지정 헤더 만들기](creating-a-custom-header-that-is-signed-and-or-encrypted.md)
### [Message 클래스 사용](using-the-message-class.md)
### [필터링](filtering.md)
### [큰 데이터 및 스트리밍](large-data-and-streaming.md)
#### [방법: 스트리밍 사용](how-to-enable-streaming.md)
### [데이터에 대한 보안 고려 사항](security-considerations-for-data.md)
### [데이터 전송 아키텍처 개요](data-transfer-architectural-overview.md)
## [세션, 인스턴스 및 동시성](sessions-instancing-and-concurrency.md)
### [방법: 세션이 필요한 서비스 만들기](how-to-create-a-service-that-requires-sessions.md)
### [방법: 서비스 인스턴스 만들기 제어](how-to-control-service-instancing.md)
### [단일 동시성 모델에서 메시지의 순서 지정 처리](ordered-processing-of-messages-in-single-concurrency-mode.md)
## [전송](transports.md)
### [전송 선택](choosing-a-transport.md)
### [메시지 인코더 선택](choosing-a-message-encoder.md)
### [스트리밍 메시지 전송](streaming-message-transfer.md)
### [HTTP 및 HTTPS 구성](configuring-http-and-https.md)
### [방법: WCF URL 예약을 제한된 예약으로 바꾸기](how-to-replace-the-wcf-url-reservation-with-a-restricted-reservation.md)
### [전송 할당량](transport-quotas.md)
### [NAT 및 방화벽 작업](working-with-nats-and-firewalls.md)
### [Net.TCP 포트 공유](net-tcp-port-sharing.md)
#### [방법: Net.TCP Port Sharing Service 사용](how-to-enable-the-net-tcp-port-sharing-service.md)
#### [방법: 포트 공유를 사용하도록 WCF 서비스 구성](how-to-configure-a-wcf-service-to-use-port-sharing.md)
#### [Net.TCP Port Sharing Service 구성](configuring-the-net-tcp-port-sharing-service.md)
### [ByteStream 인코더를 사용하여 이진 개체 인코딩](encoding-binary-objects-with-bytestream-encoder.md)
## [큐 및 신뢰할 수 있는 세션](queues-and-reliable-sessions.md)
### [신뢰할 수 있는 세션](reliable-sessions.md)
#### [신뢰할 수 있는 세션 개요](reliable-sessions-overview.md)
#### [방법: 신뢰할 수 있는 세션 내에서 메시지 교환](how-to-exchange-messages-within-a-reliable-session.md)
#### [방법: 신뢰할 수 있는 세션 내에서 메시지 보안](how-to-secure-messages-within-reliable-sessions.md)
#### [방법: HTTPS를 사용하여 신뢰할 수 있는 사용자 지정 세션 바인딩 만들기](how-to-create-a-custom-reliable-session-binding-with-https.md)
#### [신뢰할 수 있는 세션을 위한 최선의 방법](best-practices-for-reliable-sessions.md)
### [WCF의 큐](queues-in-wcf.md)
#### [큐 개요](queues-overview.md)
#### [WCF의 큐](queuing-in-wcf.md)
##### [서비스 끝점 및 큐 주소 지정](service-endpoints-and-queue-addressing.md)
##### [대기 중인 응용 프로그램 웹 호스팅](web-hosting-a-queued-application.md)
#### [방법: 대기 중인 메시지와 WCF 끝점 교환](how-to-exchange-queued-messages-with-wcf-endpoints.md)
#### [방법: WCF 끝점 및 메시지 큐 응용 프로그램과 메시지 교환](how-to-exchange-messages-with-wcf-endpoints-and-message-queuing-applications.md)
#### [세션의 대기 중인 메시지 그룹화](grouping-queued-messages-in-a-session.md)
#### [트랜잭션에서 메시지 일괄 처리](batching-messages-in-a-transaction.md)
#### [배달 못 한 편지 큐를 사용하여 메시지 전송 오류 처리](using-dead-letter-queues-to-handle-message-transfer-failures.md)
#### [포이즌 메시지 처리](poison-message-handling.md)
#### [Windows Vista, Windows Server 2003 및 Windows XP의 큐 기능 차이점](diff-in-queue-in-vista-server-2003-windows-xp.md)
#### [전송 보안을 사용하여 메시지에 보안 설정](securing-messages-using-transport-security.md)
#### [메시지 보안을 사용하여 메시지에 보안 설정](securing-messages-using-message-security.md)
#### [대기 중인 메시지 문제 해결](troubleshooting-queued-messaging.md)
#### [대기 중인 통신을 위한 최선의 방법](best-practices-for-queued-communication.md)
## [트랜잭션](transactions-in-wcf.md)
### [Windows Communication Foundation 트랜잭션 개요](transactions-overview.md)
### [트랜잭션 모델](transaction-models.md)
### [System.ServiceModel의 트랜잭션 지원](transactional-support-in-system-servicemodel.md)
#### [ServiceModel 트랜잭션 특성](servicemodel-transaction-attributes.md)
#### [ServiceModel 트랜잭션 구성](servicemodel-transaction-configuration.md)
#### [트랜잭션 흐름 사용](enabling-transaction-flow.md)
#### [방법: 트랜잭션 서비스 만들기](how-to-create-a-transactional-service.md)
#### [트랜잭션 응용 프로그램 진단](diagnosing-transactional-applications.md)
#### [COM+ 및 ServiceModel의 트랜잭션 비교](comparing-transactions-in-com-and-servicemodel.md)
#### [엔터프라이즈 서비스 트랜잭션 구성 요소 통합](integrating-enterprise-services-transactional-components.md)
### [WS-AtomicTransaction 사용](using-ws-atomictransaction.md)
#### [WS-Atomic Transaction 지원 구성](configuring-ws-atomic-transaction-support.md)
## [보안](security.md)
### [보안 개요](security-overview.md)
### [보안 개념](security-concepts.md)
#### [WCF에서 사용되는 보안 개념](security-concepts-used-in-wcf.md)
#### [분산 응용 프로그램 보안](distributed-application-security.md)
#### [보안 용어](wcf-security-terminology.md)
### [일반적인 보안 시나리오](common-security-scenarios.md)
#### [보안이 설정되지 않은 인터넷 클라이언트 및 서비스](internet-unsecured-client-and-service.md)
#### [보안이 설정되지 않은 인트라넷 클라이언트 및 서비스](intranet-unsecured-client-and-service.md)
#### [익명 클라이언트를 사용하는 전송 보안](transport-security-with-an-anonymous-client.md)
#### [기본 인증을 사용하는 전송 보안](transport-security-with-basic-authentication.md)
#### [Windows 인증을 사용하는 전송 보안](transport-security-with-windows-authentication.md)
#### [인증서 인증을 사용하는 전송 보안](transport-security-with-certificate-authentication.md)
#### [익명 클라이언트를 사용하는 메시지 보안](message-security-with-an-anonymous-client.md)
#### [사용자 이름 클라이언트를 사용하는 메시지 보안](message-security-with-a-user-name-client.md)
#### [인증서 클라이언트를 사용하는 메시지 보안](message-security-with-a-certificate-client.md)
#### [Windows 클라이언트를 사용하는 메시지 보안](message-security-with-a-windows-client.md)
#### [자격 증명 협상 없이 Windows 클라이언트를 사용하는 메시지 보안](message-security-with-a-windows-client-without-credential-negotiation.md)
#### [상호 인증서를 사용하는 메시지 보안](message-security-with-mutual-certificates.md)
#### [발급된 토큰을 사용하는 메시지 보안](message-security-with-issued-tokens.md)
#### [신뢰할 수 있는 하위 시스템](trusted-subsystem.md)
### [보안 동작](security-behaviors-in-wcf.md)
### [바인딩 및 보안](bindings-and-security.md)
#### [사용자 지정 바인딩을 사용하는 보안 기능](security-capabilities-with-custom-bindings.md)
##### [SecurityBindingElement 인증 모드](securitybindingelement-authentication-modes.md)
##### [방법: SecurityBindingElement를 사용하여 사용자 지정 바인딩 만들기](how-to-create-a-custom-binding-using-the-securitybindingelement.md)
##### [방법: 지정된 인증 모드에 대한 SecurityBindingElement 만들기](how-to-create-a-securitybindingelement-for-a-specified-authentication-mode.md)
##### [방법: WSFederationHttpBinding에서 보안 세션을 사용하지 않도록 설정](how-to-disable-secure-sessions-on-a-wsfederationhttpbinding.md)
##### [방법: 메시지 재생을 검색하도록 설정](how-to-enable-message-replay-detection.md)
##### [방법: 지원하는 자격 증명 만들기](how-to-create-a-supporting-credential.md)
##### [방법: 서명 확인 설정](how-to-set-up-a-signature-confirmation.md)
##### [방법: 최대 클럭 오차 설정](how-to-set-a-max-clock-skew.md)
##### [방법: 디지털 서명을 암호화하지 않도록 설정](how-to-disable-encryption-of-digital-signatures.md)
### [서비스 및 클라이언트에 보안 설정](securing-services-and-clients.md)
#### [WCF 보안 프로그래밍](programming-wcf-security.md)
##### [자격 증명 형식 선택](selecting-a-credential-type.md)
##### [방법: 사용자 이름 및 암호를 사용하여 인증](how-to-authenticate-with-a-user-name-and-password.md)
#### [전송 보안](transport-security.md)
##### [전송 보안 개요](transport-security-overview.md)
##### [HTTP 전송 보안](http-transport-security.md)
##### [HTTP 인증 이해](understanding-http-authentication.md)
##### [전송 보안을 통해 가장 사용](using-impersonation-with-transport-security.md)
##### [방법: SSL 인증서로 포트 구성](how-to-configure-a-port-with-an-ssl-certificate.md)
##### [방법: SSL을 사용하여 IIS에서 호스트되는 WCF 서비스 구성](how-to-configure-an-iis-hosted-wcf-service-with-ssl.md)
#### [메시지 보안](message-security-in-wcf.md)
##### [방법: X.509 인증서를 사용하여 서비스에 보안 설정](how-to-secure-a-service-with-an-x-509-certificate.md)
##### [방법: 전송 보안 및 메시지 자격 증명 사용](how-to-use-transport-security-and-message-credentials.md)
##### [WCF 서비스가 웹 팜에서 호스트될 경우 재생 공격 방지](preventing-replay-attacks-when-a-wcf-service-is-hosted-in-a-web-farm.md)
#### [보안 세션](secure-sessions.md)
##### [보안 대화 및 보안 세션](secure-conversations-and-secure-sessions.md)
##### [방법: 보안 세션 만들기](how-to-create-a-secure-session.md)
##### [방법: 보안 세션에 대한 보안 컨텍스트 토큰 만들기](how-to-create-a-security-context-token-for-a-secure-session.md)
##### [보안 세션에 대한 보안 고려 사항](security-considerations-for-secure-sessions.md)
#### [인증서 작업](working-with-certificates.md)
##### [방법: 인증서 가져오기](how-to-obtain-a-certificate-wcf.md)
##### [방법: MMC 스냅인을 사용하여 인증서 보기](how-to-view-certificates-with-the-mmc-snap-in.md)
##### [방법: 인증서의 지문 검색](how-to-retrieve-the-thumbprint-of-a-certificate.md)
##### [방법: WCF에서 X.509 인증서에 액세스할 수 있도록 설정](how-to-make-x-509-certificates-accessible-to-wcf.md)
##### [방법: 개발 중 사용할 임시 인증서 만들기](how-to-create-temporary-certificates-for-use-during-development.md)
##### [방법: 서명을 확인하는 데 사용되는 인증 기관 인증서 체인 지정](specify-the-certificate-authority-chain-verify-signatures-wcf.md)
##### [HTTPS, TCP를 통한 SSL 및 SOAP 보안의 인증서 유효성 검사 차이점](cert-val-diff-https-ssl-over-tcp-and-soap.md)
##### [Internet Explorer와 WCF로 완료된 서비스 인증서 유효성 검사의 차이점](diff-service-certificate-validation-ie-and-wcf.md)
##### [방법: 일관성 있게 X.509 인증서 참조](how-to-consistently-reference-x-509-certificates.md)
### [인증](authentication-in-wcf.md)
#### [방법: ASP.NET 멤버 자격 공급자 사용](how-to-use-the-aspnet-membership-provider.md)
#### [방법: 사용자 지정 사용자 이름 및 암호 유효성 검사기 사용](how-to-use-a-custom-user-name-and-password-validator.md)
#### [방법: 동일한 형식의 여러 보안 토큰 사용](how-to-use-multiple-security-tokens-of-the-same-type.md)
#### [서비스 ID 및 인증](service-identity-and-authentication.md)
#### [보안 협상 및 시간 제한](security-negotiation-and-timeouts.md)
#### [Windows 인증 오류 디버깅](debugging-windows-authentication-errors.md)
#### [WCF와 함께 여러 인증 스키마 사용](using-multiple-authentication-schemes-with-wcf.md)
### [권한 부여](authorization-in-wcf.md)
#### [Access Control 메커니즘](access-control-mechanisms.md)
#### [방법: 서비스에서 ASP.NET 역할 공급자 사용](how-to-use-the-aspnet-role-provider-with-a-service.md)
#### [방법: 서비스에서 ASP.NET 권한 부여 관리자 역할 공급자 사용](how-to-use-the-aspnet-authorization-manager-role-provider-with-a-service.md)
#### [ID 모델을 사용하여 클레임 및 권한 부여 관리](managing-claims-and-authorization-with-the-identity-model.md)
##### [클레임 및 토큰](claims-and-tokens.md)
##### [클레임 및 리소스 액세스 거부](claims-and-denying-access-to-resources.md)
##### [클레임 만들기 및 리소스 값](claim-creation-and-resource-values.md)
#### [위임 및 가장](delegation-and-impersonation-with-wcf.md)
### [페더레이션 및 발급된 토큰](federation-and-issued-tokens.md)
#### [페더레이션](federation.md)
#### [페더레이션 및 트러스트](federation-and-trust.md)
#### [방법: 페더레이션 클라이언트 만들기](how-to-create-a-federated-client.md)
#### [방법: 페더레이션 서비스에서 자격 증명 구성](how-to-configure-credentials-on-a-federation-service.md)
#### [방법: WSFederationHttpBinding 만들기](how-to-create-a-wsfederationhttpbinding.md)
#### [방법: 보안 토큰 서비스 만들기](how-to-create-a-security-token-service.md)
#### [SAML(Security Assertions Markup Language) 토큰 및 클레임](saml-tokens-and-claims.md)
#### [방법: 로컬 발급자 구성](how-to-configure-a-local-issuer.md)
#### [방법: 이중 페더레이션 바인딩 만들기](how-to-create-a-duplex-federated-binding.md)
### [감사](auditing-security-events.md)
#### [방법: 보안 이벤트 감사](how-to-audit-wcf-security-events.md)
### [보안 지침 및 최선의 방법](security-guidance-and-best-practices.md)
#### [보안을 위한 최선의 방법](best-practices-for-security-in-wcf.md)
#### [보안 고려 사항](security-considerations-in-wcf.md)
##### [정보 공개](information-disclosure.md)
##### [권한 상승](elevation-of-privilege.md)
##### [서비스 거부](denial-of-service.md)
##### [변조](tampering.md)
##### [재생 공격](replay-attacks.md)
##### [지원되지 않는 시나리오](unsupported-scenarios.md)
#### [성능 고려 사항](performance-considerations.md)
##### [ClaimSet에서 클레임 찾기](finding-claims-in-a-claimset.md)
##### [디지털 서명의 암호화](encryption-of-digital-signatures.md)
### [인증에 대한 확장된 보호 개요](extended-protection-for-authentication-overview.md)
#### [인증에 대한 확장된 보호 ReadMe 샘플](readme-for-extended-protection-authentication-sample.md)
## [피어 투 피어 네트워킹](peer-to-peer-networking.md)
### [피어 채널 시나리오](peer-channel-scenarios.md)
### [피어 채널 개념](peer-channel-concepts.md)
#### [피어 메시](peer-meshes.md)
#### [피어 노드](peer-nodes.md)
#### [피어 채널 보안](peer-channel-security.md)
#### [피어 확인자](peer-resolvers.md)
##### [CustomPeerResolverService: 클라이언트 등록 내부](inside-the-custompeerresolverservice-client-registrations.md)
### [피어 채널 응용 프로그램 빌드](building-a-peer-channel-application.md)
#### [NetTcpBinding 응용 프로그램을 피어 채널 응용 프로그램으로 변환](converting-a-nettcpbinding-application-to-a-peer-channel-application.md)
#### [메시지 분포 제한](limiting-message-distribution.md)
#### [온라인 및 오프라인 상태 추가](adding-online-and-offline-status.md)
#### [피어 채널 응용 프로그램 보안](securing-peer-channel-applications.md)
## [메타데이터](metadata.md)
### [메타데이터 아키텍처 개요](metadata-architecture-overview.md)
### [메타데이터 형식](metadata-formats.md)
### [메타데이터 내보내기 및 가져오기](exporting-and-importing-metadata.md)
#### [방법: 서비스 끝점으로 메타데이터 가져오기](how-to-import-metadata-into-service-endpoints.md)
#### [방법: 서비스 끝점에서 메타데이터 내보내기](how-to-export-metadata-from-service-endpoints.md)
#### [ServiceDescription 및 WSDL 참조](servicedescription-and-wsdl-reference.md)
#### [방법: Svcutil.exe를 사용하여 컴파일된 서비스 코드에서 메타데이터 내보내](how-to-use-svcutil-exe-to-export-metadata-from-compiled-service-code.md)기
### [메타데이터 게시](publishing-metadata.md)
#### [방법: 구성 파일을 사용하여 서비스의 메타데이터 게시](how-to-publish-metadata-for-a-service-using-a-configuration-file.md)
#### [방법: 코드를 사용하여 서비스에 대한 메타데이터 게시](how-to-publish-metadata-for-a-service-using-code.md)
### [메타데이터 검색](retrieving-metadata.md)
#### [방법: Svcutil.exe를 사용하여 메타데이터 문서 다운로드](how-to-use-svcutil-exe-to-download-metadata-documents.md)
#### [방법: MetadataResolver를 사용하여 동적으로 바인딩 메타데이터 가져오기](how-to-use-metadataresolver-to-obtain-binding-metadata-dynamically.md)
#### [방법: MetadataExchangeClient를 사용하여 메타데이터 검색](how-to-use-metadataexchangeclient-to-retrieve-metadata.md)
### [메타데이터 사용](using-metadata.md)
#### [생성된 클라이언트 코드 이해](understanding-generated-client-code.md)
#### [방법: 메타데이터 검색 및 규격 서비스 구현](how-to-retrieve-metadata-and-implement-a-compliant-service.md)
#### [서비스 메타데이터에서 WCF 클라이언트 생성](generating-a-wcf-client-from-service-metadata.md)
### [메타데이터 관련 보안 고려 사항](security-considerations-with-metadata.md)
#### [방법: 메타데이터 끝점 보안 설정](how-to-secure-metadata-endpoints.md)
#### [방법: 권한을 부여하는 동안 메타데이터 요청 허용](how-to-allow-metadata-requests-while-authorizing.md)
## [클라이언트](clients.md)
### [WCF 클라이언트 아키텍처](client-architecture.md)
### [WCF 클라이언트를 사용하여 서비스 액세스](accessing-services-using-a-client.md)
#### [방법: 단방향 및 요청-회신 계약을 사용하여 서비스 액세스](how-to-access-wcf-services-with-one-way-and-request-reply-contracts.md)
#### [방법: 이중 계약을 사용하여 서비스 액세스](how-to-access-services-with-a-duplex-contract.md)
#### [방법: WSE 3.0 서비스 액세스](how-to-access-a-wse-3-0-service-with-a-wcf-client.md)
#### [방법: ChannelFactory 사용](how-to-use-the-channelfactory.md)
#### [채널 팩터리 및 캐싱](channel-factory-and-caching.md)
#### [방법: 비동기적으로 서비스 작업 호출](how-to-call-wcf-service-operations-asynchronously.md)
#### [중간 계층 클라이언트 응용 프로그램](middle-tier-client-applications.md)
#### [방법: 채널 팩터리를 사용하여 비동기로 작업 호출](how-to-call-operations-asynchronously-using-a-channel-factory.md)
#### [Windows 스토어 클라이언트 응용 프로그램을 사용하여 WCF 서비스에 액세](accessing-wcf-services-with-a-windows-store-client-app.md)스
#### [방법: 채널 팩터리를 만들어 채널을 만들고 관리하는 데 사용](how-to-create-a-channel-factory-and-use-it-to-create-and-manage-channels.md)
### [WCF 클라이언트 구성](client-configuration.md)
## [호스팅](hosting.md)
### [인터넷 정보 서비스에서 호스팅](hosting-in-internet-information-services.md)
#### [인터넷 정보 서비스에서 호스트하는 WCF 서비스 배포](deploying-an-internet-information-services-hosted-wcf-service.md)
#### [WCF 서비스 및 ASP.NET](wcf-services-and-aspnet.md)
#### [인터넷 정보 서비스 호스팅을 위한 최선의 방법](internet-information-services-hosting-best-practices.md)
#### [방법: IIS에서 WCF 서비스 호스트](how-to-host-a-wcf-service-in-iis.md)
#### [Windows Communication Foundation에 대해 Internet Information Services 7.0 구성](configuring-iis-for-wcf.md)
### [Windows Process Activation Service에서 호스팅](hosting-in-windows-process-activation-service.md)
#### [WAS Activation 아키텍처](was-activation-architecture.md)
#### [WCF와 함께 사용하도록 WAS 구성](configuring-the-wpa--service-for-use-with-wcf.md)
#### [방법: WCF Activation 구성 요소 설치 및 구성](how-to-install-and-configure-wcf-activation-components.md)
#### [방법: WAS에서 WCF 서비스 호스트](how-to-host-a-wcf-service-in-was.md)
### [Windows 서비스 응용 프로그램에서의 호스팅](hosting-in-a-windows-service-application.md)
#### [방법: 관리되는 Windows 서비스에서 WCF 서비스 호스팅](how-to-host-a-wcf-service-in-a-managed-windows-service.md)
### [관리되는 응용 프로그램에서의 호스팅](hosting-in-a-managed-application.md)
### [IIS 및 WAS에서 구성 기반 활성화](configuration-based-activation-in-iis-and-was.md)
### [여러 IIS 사이트 바인딩 지원](supporting-multiple-iis-site-bindings.md)
### [System.Web.Routing 통합](system-web-routing-integration.md)
## [부분 신뢰](partial-trust.md)
### [지원되는 배포 시나리오](supported-deployment-scenarios.md)
### [부분 신뢰 기능 호환성](partial-trust-feature-compatibility.md)
### [부분 신뢰를 위한 최선의 방법](partial-trust-best-practices.md)
## [상호 운용성 및 통합](interoperability-and-integration.md)
### [웹 서비스 프로토콜 상호 운용성 가이드](web-services-protocols-interoperability-guide.md)
#### [시스템 제공 상호 운용성 바인딩에서 지원하는 웹 서비스 프로토콜](web-services-protocols-supported-by-system-provided-interoperability-bindings.md)
#### [메시징 프로토콜](messaging-protocols.md)
#### [데이터 계약 스키마 참조](data-contract-schema-reference.md)
#### [WSDL 및 정책](wsdl-and-policy.md)
#### [보안 프로토콜 버전 1.0](security-protocols-version-1-0.md)
#### [보안 프로토콜](security-protocols.md)
#### [Reliable Messaging 프로토콜 버전 1.0](reliable-messaging-protocol-version-1-0.md)
#### [Reliable Messaging 프로토콜 버전 1.1](reliable-messaging-protocol-version-1-1.md)
#### [트랜잭션 프로토콜 버전 1.0](transaction-protocols-version-1-0.md)
#### [트랜잭션 프로토콜](transaction-protocols.md)
#### [컨텍스트 교환 프로토콜](context-exchange-protocol.md)
#### [페더레이션 시나리오에서 트러스트 프로토콜 혼합](mixing-trust-protocols-in-federated-scenarios.md)
### [COM+ 응용 프로그램과 통합](integrating-with-com-plus-applications.md)
#### [COM+ 응용 프로그램과 통합 개요](integrating-with-com-plus-applications-overview.md)
#### [방법: COM+ 서비스 모델 구성 도구 사용](how-to-use-the-com-service-model-configuration-tool.md)
#### [방법: COM+ 서비스 설정 구성](how-to-configure-com-service-settings.md)
#### [방법: COM+ 통합 응용 프로그램 배포](how-to-deploy-a-com-integration-application.md)
### [COM 응용 프로그램과 통합](integrating-with-com-applications.md)
#### [COM 응용 프로그램과 통합 개요](integrating-with-com-applications-overview.md)
#### [방법: 서비스 모니커 등록 및 구성](how-to-register-and-configure-a-service-moniker.md)
#### [방법: 등록 없이 Windows Communication Foundation 서비스 모니커 사용](use-the-wcf-service-moniker-without-registration.md)
#### [방법: WSDL 계약을 통해 서비스 모니커 사용](how-to-use-a-service-moniker-with-wsdl-contracts.md)
#### [방법: 메타데이터 교환 계약을 통해 서비스 모니커 사용](how-to-use-a-service-moniker-with-metadata-exchange-contracts.md)
#### [방법: 채널 보안 자격 증명 지정](how-to-specify-channel-security-credentials.md)
### [.NET Remoting 응용 프로그램을 WCF로 마이그레이션](migrating-net-remoting-applications-to-wcf.md)
### [Web Services Enhancements 3.0과의 상호 운용성](interoperability-with-web-services-enhancements-3-0.md)
#### [방법: WSE 3.0 클라이언트와 상호 운용하도록 WCF 서비스 구성](how-to-configure-wcf-services-to-interoperate-with-wse-3-0-clients.md)
#### [방법: WSE3.0 서비스와 상호 운용하도록 WCF 클라이언트 구성](how-to-configure-a-wcf-client-to-interoperate-with-wse3-0-services.md)
### [WSE 3.0 웹 서비스를 WCF로 마이그레이션](migrating-wse-3-0-web-services-to-wcf.md)
### [ASP.NET 웹 서비스와의 상호 운용성](interop-with-aspnet-web-services.md)
#### [방법: ASP.NET 웹 서비스 클라이언트와 상호 운용하도록 WCF 서비스 구성](config-wcf-service-with-aspnet-web-service.md)
### [ASP.NET 웹 서비스를 WCF로 마이그레이션](migrating-aspnet-web-services-to-wcf.md)
#### [용도와 사용되는 표준을 기반으로 ASP.NET 웹 서비스와 WCF 비교](comparing-aspnet-web-services-to-wcf-based-on-purpose-and-standards-used.md)
#### [개발을 기반으로 ASP.NET 웹 서비스와 WCF 비교](comparing-aspnet-web-services-to-wcf-based-on-development.md)
#### [Windows Communication Foundation 채택 예상: 이후의 통합을 용이하게 함](anticipating-adopting-the-wcf-easing-future-integration.md)
#### [Windows Communication Foundation 채택 예상: 이후의 마이그레이션을 용이하게 함](anticipating-adopting-wcf-migration.md)
#### [Windows Communication Foundation 채택](adopting-wcf.md)
##### [방법: ASP.NET 웹 서비스 코드를 Windows Communication Foundation으로 마이그레이션](migrate-asp-net-web-service-to-wcf.md)
##### [방법: ASP.NET 웹 서비스 클라이언트 코드를 Windows Communication Foundation으로 마이그레이션](migrate-asp-net-web-service-client-to-wcf.md)
### [POX 응용 프로그램과의 상호 운용성](interoperability-with-pox-applications.md)
## [WCF 웹 HTTP 프로그래밍 모델](wcf-web-http-programming-model.md)
### [WCF 웹 HTTP 프로그래밍 모델 개요](wcf-web-http-programming-model-overview.md)
### [WCF 웹 HTTP 프로그래밍 개체 모델](wcf-web-http-programming-object-model.md)
### [방법: 기본 WCF 웹 HTTP 서비스 만들기](how-to-create-a-basic-wcf-web-http-service.md)
### [방법: SOAP 및 웹 클라이언트에 계약 공개](how-to-expose-a-contract-to-soap-and-web-clients.md)
### [UriTemplate 및 UriTemplateTable](uritemplate-and-uritemplatetable.md)
### [방법: WCF 웹 HTTP 프로그래밍 모델을 사용하여 임의의 데이터를 반환하는 서비스 만들기](service-returns-arbitrary-data-using-the-wcf-web.md)
### [방법: WCF REST 프로그래밍 모델을 사용하여 임의의 데이터를 허용하는 서비스 만들기](create-a-service-arbitrary-data-using-wcf.md)
### [WCF 웹 HTTP 서비스에 대한 캐싱 지원](caching-support-for-wcf-web-http-services.md)
### [WCF 웹 HTTP 서비스 도움말 페이지](wcf-web-http-service-help-page.md)
### [WCF 웹 HTTP 형식 지정](wcf-web-http-formatting.md)
### [WCF 웹 HTTP 오류 처리](wcf-web-http-error-handling.md)
### [JSONP 사용](using-jsonp.md)
### [WCF 서비스에서 REST 스타일 서비스 호출](calling-a-rest-style-service-from-a-wcf-service.md)
## [WCF 배포](wcf-syndication.md)
### [WCF 배포 개요](wcf-syndication-overview.md)
### [배포 아키텍처](architecture-of-syndication.md)
### [WCF 배포 개체 모델을 Atom 및 RSS로 매핑하는 방법](how-the-wcf-syndication-object-model-maps-to-atom-and-rss.md)
### [방법: 기본 RSS 피드 만들기](how-to-create-a-basic-rss-feed.md)
### [방법: 기본 Atom 피드 만들기](how-to-create-a-basic-atom-feed.md)
### [방법: Atom 및 RSS로 피드 공개](how-to-expose-a-feed-as-both-atom-and-rss.md)
### [배포 확장성](syndication-extensibility.md)
## [AJAX 통합 및 JSON 지원](ajax-integration-and-json-support.md)
### [ASP.NET AJAX용 WCF 서비스 만들기](creating-wcf-services-for-aspnet-ajax.md)
#### [방법: AJAX 사용 WCF 서비스 만들기 및 액세스](create-an-ajax-wcf-asp-net-client.md)
#### [방법: 구성을 사용하지 않고 ASP.NET AJAX 끝점 추가](how-to-add-an-aspnet-ajax-endpoint-without-using-configuration.md)
#### [방법: 구성을 사용하여 ASP.NET AJAX 끝점 추가](how-to-use-configuration-to-add-an-aspnet-ajax-endpoint.md)
#### [방법: ASP.NET AJAX 끝점에 대해 HTTP POST 및 HTTP GET 요청 중에서 선택](http-post-and-http-get-requests-for-aspnet-ajax-endpoints.md)
### [ASP.NET을 사용하지 않고 WCF AJAX 서비스 만들기](creating-wcf-ajax-services-without-aspnet.md)
### [JSON 및 기타 데이터 전송 형식에 대한 지원](support-for-json-and-other-data-transfer-formats.md)
#### [독립 실행형 JSON Serialization](stand-alone-json-serialization.md)
#### [방법: JSON 데이터 Serialize 및 Deserialize](how-to-serialize-and-deserialize-json-data.md)
#### [JSON과 XML 간의 매핑](mapping-between-json-and-xml.md)
#### [메시지 수준의 프로그래밍으로 JSON으로 serialize](serializing-in-json-with-message-level-programming.md)
### [방법: AJAX 사용 ASP.NET 웹 서비스를 WCF로 마이그레이션](how-to-migrate-ajax-enabled-aspnet-web-services-to-wcf.md)
## [WCF 검색](wcf-discovery.md)
### [WCF 검색 개요](wcf-discovery-overview.md)
### [WCF 검색 개체 모델](wcf-discovery-object-model.md)
### [검색 찾기 및 FindCriteria](discovery-find-and-findcriteria.md)
### [방법: 프로그래밍 방식으로 WCF 서비스 및 클라이언트에 검색 기능 추가](how-to-programmatically-add-discoverability-to-a-wcf-service-and-client.md)
### [검색 프록시 구현](implementing-a-discovery-proxy.md)
#### [방법: 검색 프록시 구현](how-to-implement-a-discovery-proxy.md)
#### [방법: 검색 프록시에 등록할 검색 가능한 서비스 구현](discoverable-service-that-registers-with-the-discovery-proxy.md)
#### [방법: 검색 프록시를 사용하여 서비스를 찾는 클라이언트 응용 프로그램 구현](client-app-discovery-proxy-to-find-a-service.md)
#### [방법: 검색 프록시 테스트](how-to-test-the-discovery-proxy.md)
#### [방법: 프로브 요청의 검색 버전 확인](how-to-determine-the-discovery-version-of-a-probe-request.md)
### [검색 버전 관리](discovery-versioning.md)
### [구성 파일에서 검색 구성](configuring-discovery-in-a-configuration-file.md)
### [검색 클라이언트 채널 사용](using-the-discovery-client-channel.md)
### [검색 클라이언트 채널을 통해 사용자 지정 바인딩 사용](using-a-custom-binding-with-the-discovery-client-channel.md)
### [검색 알림 및 알림 클라이언트](discovery-announcements-and-announcement-client.md)
### [DiscoveryClient 및 DynamicEndpoint](discoveryclient-and-dynamicendpoint.md)
## [라우팅](routing.md)
### [라우팅 소개](routing-introduction.md)
### [라우팅 서비스](routing-service.md)
### [라우팅 계약](routing-contracts.md)
### [메시지 필터](message-filters.md)
#### [필터 선택](choosing-a-filter.md)
#### [사용자 지정 필터](custom-filters.md)
#### [방법: 필터 사용](how-to-use-filters.md)
### [라우팅 시나리오](routing-scenarios.md)
#### [방법: 서비스 버전 관리](how-to-service-versioning.md)
#### [방법: 서비스 데이터 분할](how-to-service-data-partitioning.md)
#### [방법: 동적 업데이트](how-to-dynamic-update.md)
#### [방법: 오류 처리](how-to-error-handling.md)
## [WCF 및 IDN(Internationalized Domain Name)](wcf-and-internationalized-domain-names.md)
## [WCF 및 WebSocket](wcf-and-websockets.md)
### [NetHttpBinding 사용](using-the-nethttpbinding.md)
### [방법: WebSocket을 통해 통신하는 WCF 서비스 만들기](how-to-create-a-wcf-service-that-communicates-over-websockets.md)
## [오류 처리](error-handling.md)
