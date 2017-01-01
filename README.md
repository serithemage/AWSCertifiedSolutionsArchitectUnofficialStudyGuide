# 비공식 AWS 공인 솔루션스 아키텍트 - 어소시에이트 수험 가이드

> 이 문서는 AWS 공인 솔루션스 아키텍트 [시험 안내서](https://d0.awsstatic.com/International/ko_KR/AWS_certified_solutions_architect_associate_blueprint_ko.pdf)에 적힌 내용에 기반하여 AWS의 홈페이지, 블로그, Slideshare의 관련 링크를 한글 자료 중심으로 정리해 놓은 것 입니다. 어소시에이트 레벨이기때문에 깊이 있는 내용을 다루지는 않습니다만 서비스의 특징과 이를 조합한 아키텍처 디자인에 대한 개념들을 파악하고 계셔야 합니다. 

> 단축URL: http://bit.ly/sacertguide

## 기본적인 시험 정보
- [시험 안내서](https://d0.awsstatic.com/International/ko_KR/AWS_certified_solutions_architect_associate_blueprint_ko.pdf): 많은 분들이 제대로 읽어보시지 않으시는데 수험 준비를 위해 대단히 중요한 문서이므로 꼼꼼히 읽어 두셔야 합니다. 이 문서는 이 시험 안내서에 기반하여 작성되었습니다.
- [시험 안내 페이지](https://aws.amazon.com/ko/certification/certified-solutions-architect-associate/)
- [시험 신청](https://www.webassessor.com/wa.do?page=publicHome&branding=AMAZON)
- [AWS기반 아키텍처 설계](https://aws.amazon.com/ko/training/course-descriptions/architect/): 3일동안 강의와 실습으로 진행되는 수업이며 이 수업에서 다루는 내용이 바로 AWS 솔루션스 아키텍트 자격증시험의 출제 범위가 됩니다.
- [시험 워크숍 참여](https://www.aws.training/home?courseid=10&&language=en-US&view=table&source=web_en_certified-sa-assoc)
- [샘플문항](https://d0.awsstatic.com/International/ko_KR/AWS_certified_solutions_architect_associate_examsample_ko.pdf): 8개의 샘플문항 입니다. 실전과 동일한 유형과 난이도를 제공합니다.
- [연습시험 응시](https://www.webassessor.com/wa.do?page=publicHome&branding=AMAZON): 20문제가 출제되고 유료(20달러) 입니다.
- [공식 수험 준비서(영문)](https://www.webassessor.com/wa.do?page=publicHome&branding=AMAZON): 킨들과 종이책 버전이 있으며 각 서비스에 대한 설명과 연습문제가 수록되어 있습니다.
- [수험 준비를 위한 자습형 실습](https://qwiklabs.com/quests/10)
- [영문 시험 시간 추가 요청 방법](http://edu.supertrack.co.kr/notice/news.php?ptype=view&idx=5177&page=1&code=news): 영문으로 시험을 보실 경우 30분 시험시간을 추가하실 수 있습니다. **주의! 반드시 시험 신청 하시기 전에 시험시간 추가 신청을 하셔야 합니다!**

## 시험 범위에 해당되는 AWS공식문서들

### 전체
- [AWS 한국어 설명서 목록](https://aws.amazon.com/ko/blogs/korea/ko-documentation/): 여기 정리된 링크들은 대부분 SA 자격시험 출제범위임.(관리자용이나 개발자용 문서는 제외)
- [AWS 한국어 기술 백서 목록](https://aws.amazon.com/ko/blogs/korea/ko-whitepapers/): 내용이 많지만 잘 정리되어 있어서 쉽게 읽힙니다.
- [AWS 아키텍처 센터](https://aws.amazon.com/ko/architecture/)


### 분야 1.0: 고가용성, 비용 효율적, 내결함성, 확장형 시스템 디자인
- [AWS Well-Architected 프레임워크](https://d0.awsstatic.com/International/ko_KR/whitepapers/Well-Architected_Whitepaper.pdf)
- [지역 및 가용영역](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)
- 클라우드 서비스를 설계하는 방법
  - [AWS 고급 아키텍처 방법론](http://www.slideshare.net/awskorea/aws-cloud-track-2-advanced)
  - [AWS 기반의 마이크로 서비스 아키텍쳐 구현 방안](http://www.slideshare.net/awskorea/micro-service-oriented-architecture-on-aws-piljoong-kim)
- 계획 및 설계
  - [클라우드를 위한 아키텍처 설계 - 모범 사례](https://amz.kr/pdf/Architecture_Best_Practices_draft-KR.pdf)
  - [AWS 고객 사례 모음](https://www.awsseoul.kr/images/content/aws-korea-customer-cases-2016.pdf) 
- 모니터링
  - [Cloudwatch](https://aws.amazon.com/ko/cloudwatch/faqs/)
  - [CloudTrail](https://aws.amazon.com/ko/cloudtrail/faqs/)
  - [Trusted Advisor](https://aws.amazon.com/ko/premiumsupport/trustedadvisor/)
  - [모니터링 모범사례](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/monitoring_best_practices.html)
- 모범 사례
  - [EC2 모범사례](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/ec2-best-practices.html)
- 가격/비용을 비롯한 클라이언트 사양 개발(예: 온디맨드 vs. 예약 vs. 스폿, RT  - 및 RP  - DR디자인)
  - [Amazon EC2 요금](https://aws.amazon.com/ko/ec2/pricing/)
- 아키텍처적 트레이드오프(고가용성과 비용 간 트레이드오프, Amazon Relational Database Service(RDS)를 사용하는 것과 Amazon Elastic Compute Cloud(EC2)에 자체 데이터베이스를 설치하는 것 간의 트레이드오프)
  - [Amazon Relational Database Service(Amazon RDS)는 무엇인가?](http://docs.aws.amazon.com/ko_kr/AmazonRDS/latest/UserGuide/Welcome.html)
- 기존 개발 환경과의 통합 및 확장형 아키텍처 구축
  - [AWS Enterprise Summit :: 하이브리드 클라우드 인프라를 통한 데이터센터 확장과 마이그레이션 방안](http://www.slideshare.net/awskorea/aws-enterprise-summit-67243885)
- 탄력성 및 확장성
  - [AWS 클라우드에서의 웹 애플리케이션 호스팅](http://d0.awsstatic.com/whitepapers/International/ko/AWS_Web_Hosting_Best_Practices_05252010.pdf)
  - [RDS의 고가용성(다중 AZ)](https://docs.aws.amazon.com/ko_kr/AmazonRDS/latest/UserGuide/Concepts.MultiAZ.html)
  - [Amazon CloudWatch를 사용하여 Auto Scaling 인스턴스 및 그룹 모니터링](http://docs.aws.amazon.com/ko_kr/autoscaling/latest/userguide/as-instance-monitoring.html)
  - [Auto Scaling 그룹에 로드 밸런서 사용](http://docs.aws.amazon.com/ko_kr/autoscaling/latest/userguide/autoscaling-load-balancer.html)

### 분야 2.0: 구현/배포 - Amazon EC2, Amazon S3, Elastic Beanstalk, CloudFormation, Amazon Virtual Private Cloud(VPC) 및 AWS Identity and Access Management(IAM)를 사용하여 클라우드 솔루션을 코딩하고 구현하기 위한 적절한 기술과 방법을 파악한다.
- [Amazon Machine Image:AMI](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/AMIs.html)
- [AWS Direct Connect](https://aws.amazon.com/ko/directconnect/)
- [AWS Stroage Gateway](https://aws.amazon.com/ko/storagegateway/)
- 개별 서비스
  - [EC2](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/concepts.html) : AWS의 핵심서비스인 만큼 EC2에 대한 내용은 무척 비중있게 다루어집니다.
    - [인스턴스 및 AMI](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/ec2-instances-and-amis.html)
    - [리전 및 가용 영역](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)
    - [Amazon EC2 루트 디바이스 볼륨](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/RootDeviceStorage.html)
    - [Amazon EC2 모니터링](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/monitoring_ec2.html)
    - [네트워크 및 보안](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EC2_Network_and_Security.html)
    - [스토리지](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/Storage.html)
    - [Auto Scaling 설명서](http://docs.aws.amazon.com/ko_kr/autoscaling/latest/userguide/WhatIsAutoScaling.html)
  - [VPC](https://aws.amazon.com/ko/vpc/faqs/)
    - [VPC 사용자 가이드](http://docs.aws.amazon.com/ko_kr/AmazonVPC/latest/UserGuide/VPC_Introduction.html)
    - [VPC 피어링이란?](http://docs.aws.amazon.com/ko_kr/AmazonVPC/latest/PeeringGuide/Welcome.html)
    - [Amazon Virtual Private Cloud 를 이용한 IT 인프라의 확장](http://d0.awsstatic.com/International/ko_KR/whitepapers/Extend%20your%20IT%20infrastructure%20with%20Amaon%20VPC.pdf)
  - [Elastic Beanstalk](https://aws.amazon.com/ko/elasticbeanstalk/faqs/)
    - [Elastic Beanstalk를 이용한 웹 앱 배포](http://docs.aws.amazon.com/ko_kr/gettingstarted/latest/deploy/overview.html)
  - [EBS](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EBSVolumes.html)
    - [EBS FAQ](https://aws.amazon.com/ko/ebs/faqs/)
    - [EBS 볼륨 유형](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EBSVolumeTypes.html)
    - [EBS 스냅샷](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EBSSnapshots.html)
    - [EBS 암호화](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EBSEncryption.html)
    - [Linux 인스턴스의 Amazon EBS 볼륨 성능](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/EBSPerformance.html)
  - [Amazon EC2 인스턴스 스토어](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/InstanceStorage.html)
  - S3
    - [Amazon S3 FAQ](https://aws.amazon.com/ko/s3/faqs/)
    - [Amazon S3 리소스에 대한 액세스 권한 관리](https://docs.aws.amazon.com/ko_kr/AmazonS3/latest/dev/s3-access-control.html)
    - [S3 스토리지 클래스](https://aws.amazon.com/ko/s3/storage-classes/)
    - [S3 Reduced Redundancy Storage](https://aws.amazon.com/ko/s3/reduced-redundancy/)
  - [CloudFormation](https://aws.amazon.com/ko/cloudformation/faqs/)
  - [OpsWorks](https://aws.amazon.com/ko/opsworks/faqs/)
  - [Amazon SNS](https://aws.amazon.com/ko/sns/faqs/)
  - [Amazon SQS](https://aws.amazon.com/ko/sqs/faqs/)
  - [AWS Storage Gateway](https://aws.amazon.com/ko/storagegateway/faqs/)
  - [Amazon DynamoDB](https://aws.amazon.com/ko/dynamodb/faqs/)
    - [SQL에서 NoSQL로](https://docs.aws.amazon.com/ko_kr/amazondynamodb/latest/developerguide/SQLtoNoSQL.html)
    - [프로비저닝된 처리량](https://docs.aws.amazon.com/ko_kr/amazondynamodb/latest/developerguide/HowItWorks.ProvisionedThroughput.html)
    - [DynamoDB의 쿼리 및 스캔 작업](https://docs.aws.amazon.com/ko_kr/amazondynamodb/latest/developerguide/QueryAndScan.html)
    - [파티션 및 데이터 배포](https://docs.aws.amazon.com/ko_kr/amazondynamodb/latest/developerguide/HowItWorks.Partitions.html)

### 분야 3.0: 데이터 보안 - 최적의 클라우드 배포 및 유지보수를 위한 보안 절차를 파악하고 구현
- [클라우드 보안 모범 사례](https://d0.awsstatic.com/International/ko_KR/whitepapers/AWS_Security_Best_Practices_11052013.pdf)
- [AWS 한글 보안 기술 백서](https://aws.amazon.com/ko/blogs/korea/aws-security-whitepapers/)
- [보안 프로세스의 개요](http://d0.awsstatic.com/International/ko_KR/whitepapers/AWS_Security_Whitepaper_Overview.pdf)
- [AWS Security by Design](http://d0.awsstatic.com/International/ko_KR/whitepapers/Compliance/Intro_to_Security_by_Design.pdf)
- [AWS IAM 모범사례](http://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/best-practices.html)
  - 책임 분담 보안 모델 ([클라우드 보안 모범 사례](https://d0.awsstatic.com/International/ko_KR/whitepapers/AWS_Security_Best_Practices_11052013.pdf) 안에 포함되어 있음)
  - AWS 플랫폼 규정 준수
    - [AWS 클라우드 규정 준수](https://aws.amazon.com/ko/compliance/)
  - AWS 보안 속성(고객 워크로드부터 물리적 계층까지)
    - [규모별 보안: AWS 기반 거버넌스](http://d0.awsstatic.com/International/ko_KR/whitepapers/Compliance/AWS_Security_at_Scale_Governance_in_AWS_Whitepaper.pdf)
    - [규모별 보안: AWS에서 로깅하기](http://d0.awsstatic.com/International/ko_KR/whitepapers/Compliance/AWS_Security_at_Scale_Logging_in_AWS_Whitepaper.pdf)
  - 보안 서비스
    - [AWS Identity and Access Management(IAM)](http://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/introduction.html)
    - [Amazon Virtual Private Cloud(VPC)](http://docs.aws.amazon.com/ko_kr/AmazonVPC/latest/UserGuide/VPC_Introduction.html)
  - CIA 및 AAA 모델, 인바운드 및 아웃바운드 필터링 그리고 이에 맞는 AWS 서비스 및 기능
  - ‘핵심’ Amazon EC2 및 S3 보안 기능 집합
    - [Amazon S3 리소스에 대한 액세스 권한 관리](https://docs.aws.amazon.com/ko_kr/AmazonS3/latest/dev/s3-access-control.html)
  - 공통적인 일반 보안 제품 통합(방화벽, IDS:HIDS/NIDS, SIEM, VPN)
  - 디자인 패턴
    - [AWS Cloud Design Patterns](http://en.clouddesignpattern.org/index.php/Main_Page)
    - [Monitoring Integration Pattern](http://en.clouddesignpattern.org/index.php/CDP:Monitoring_Integration_Pattern)
  - DDos 완화
    - [DDoS 대응을 위한 AWS 모범사례](https://d0.awsstatic.com/International/ko_KR/whitepapers/DDoS_White_Paper.pdf)
  - [암호화 솔루션](http://d0.awsstatic.com/International/ko_KR/whitepapers/Compliance/AWS_Securing_Data_at_Rest_with_Encryption.pdf)
  - 정교한 액세스 제어(세밀한 보안 그룹, ACL 등 구축)
    - [VPC의 보안그룹](http://docs.aws.amazon.com/ko_kr/AmazonVPC/latest/UserGuide/VPC_SecurityGroups.html)
    - [네트워크 ACL](http://docs.aws.amazon.com/ko_kr/AmazonVPC/latest/UserGuide/VPC_ACLs.html)
  - [보안 아키텍트를 위한 Amazon CloudWatch](https://aws.amazon.com/ko/cloudwatch/details/)
- [AWS를 사용하는 백업 및 복구 접근 방식](https://d0.awsstatic.com/whitepapers/Storage/LocalizedBR/Backup_and_Recovery_Approaches_Using_AWS_whitepaper_KR.pdf)
- [AWS Import/Export](https://aws.amazon.com/ko/documentation/importexport/?nc1=h_ls)
- [AWS Storage Gateway](https://aws.amazon.com/ko/storagegateway/details/)
- [AWS Directory Service](https://aws.amazon.com/ko/directoryservice/faqs/)
- [Amazon Route53](https://aws.amazon.com/ko/route53/details/)
- [Amazon CloudFront](https://docs.aws.amazon.com/ko_kr/AmazonCloudFront/latest/DeveloperGuide/Introduction.html)
- [Amazon S3에서 CloudFront 사용](http://docs.aws.amazon.com/ko_kr/AmazonCloudFront/latest/DeveloperGuide/MigrateS3ToCloudFront.html)

### 분야 4.0: 문제 해결
> 이 영역은 대부분 각 서비스의 FAQ와 관련이 있습니다.

- 일반적인 문제 해결 정보 및 질문
  - [인스턴스 연결 중 오류 발생: 연결시간 초과](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/TroubleshootingInstancesConnecting.html#TroubleshootingInstancesConnectionTimeout)
  - [인스턴스 문제 해결](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/ec2-instance-troubleshoot.html)
  - [IAM 문제 해결](http://docs.aws.amazon.com/ko_kr/IAM/latest/UserGuide/troubleshoot.html)
- [AWS Service Limits](http://docs.aws.amazon.com/ko_kr/general/latest/gr/aws_service_limits.html): AWS에는 요청으로 변경 가능한 제한(Soft Limits)과 변경이 불가능한 제한(Hard Limits)이 있습니다.
  - [Amazon EC2 서비스 제한](http://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/ec2-resource-limits.html) 
- [Amazon EC2 인스턴스 FAQ](https://aws.amazon.com/ko/instance-help/)
