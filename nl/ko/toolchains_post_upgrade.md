---

copyright:
  years: 2015, 2017
lastupdated: "2017-8-17"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# {{site.data.keyword.jazzhub_short}} 프로젝트 업그레이드 후 도구 체인 시작하기
{: #toolchains_post_upgrade}

hub.jazz.net의 {{site.data.keyword.jazzhub}} 프로젝트가 IBM Bluemix {{site.data.keyword.contdelivery_short}} 서비스에서 도구 체인으로 업그레이드되었습니다.  

hub.jazz.net의 {{site.data.keyword.jazzhub_short}}가 취소됩니다.  

DevOps 프로젝트의 경우 [{{site.data.keyword.contdelivery_short}} 서비스![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.bluemix.net/devops){:new_window}를 참조하십시오. {{site.data.keyword.Bluemix_notm}}를 처음 사용하는 경우 [Bluemix 개요](/docs/overview/whatisbluemix.html#bluemixoverview)를 확인하십시오.

{: shortdesc}

## 프로젝트에서 작성된 도구 체인 찾기
{: #find_toolchain}

[도구 체인 페이지![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.bluemix.net/devops/toolchains){: new_window}로 이동하고 hub.jazz.net 프로젝트의 이름과 일치하는 이름으로 도구 체인이 표시되는지 확인하여 업그레이드가 완료되었음을 확인하십시오. 프로젝트가 자동으로 업그레이드된 경우 다음 제한사항에 유의하십시오. 
   - 프로젝트가 업그레이드되기 전에 다른 도구 체인에서 이미 프로젝트의 이름을 사용한 경우 프로젝트에 대해 작성된 새 도구 체인의 이름은 프로젝트의 이름과 일치하면 안 됩니다.  
   - 프로젝트에 대한 도구 체인이 표시되지 않으면 속해 있는 다른 조직으로 전환하고 도구 체인을 확인하십시오. 
   - 프로젝트에 대한 도구 체인을 계속해서 찾을 수 없으면 업그레이드가 진행 중일 수 있습니다. 도구 체인에 즉시 액세스해야 하는 경우 [지원 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://developer.ibm.com/answers/questions/ask/?smartspace=devops-services){:new_window}에 문의하십시오.

## 도구 체인 개요
{: #compare_toolchains}

hub.jazz.net에 하나 이상의 프로젝트가 있으면 {{site.data.keyword.contdelivery_short}} 서비스에서 도구 체인으로 업그레이드된 것입니다. 프로젝트에 대한 도구 체인이 표시되지 않으며 도구 체인에 즉시 액세스해야 하는 경우 [지원![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://developer.ibm.com/answers/questions/ask/?smartspace=devops-services){:new_window}을 참조하십시오. 

도구 체인은 프로젝트와 유사하지만 일부 중요한 차이점이 있습니다. 

- 프로젝트에는 오직 하나의 저장소(repo)와 파이프라인만 있을 수 있습니다. 도구 체인에는 필요한 수 만큼의 저장소와 파이프라인이 있을 수 있습니다. 
- 도구 체인에는 프로젝트에서 사용 가능하지 않은 도구가 포함될 수 있습니다(예: Slack, Sauce Labs, PagerDuty 및 {{site.data.keyword.DRA_full}}). 
- 프로젝트에서 멤버십은 프로젝트 레벨로 유지됩니다. 도구 체인에 대한 액세스는 {{site.data.keyword.Bluemix_notm}} 조직 및 도구 체인으로 관리됩니다. 도구 체인에 대해 작업하려면 도구 체인이 포함된 조직의 구성원이어야 합니다. 도구 체인 소유자는 도구 체인에 액세스할 수 있는 사용자 및 수행할 수 있는 작업을 추가로 제어할 수 있습니다. 세부사항은 [도구 체인 시작하기](#upgrade_next_steps)에 있는 단계 2를 참조하십시오.
- hub.jazz.net의 프로젝트에 사용한 저장소의 유형에 따라 도구 체인에는 GitHub.com 저장소 또는 {{site.data.keyword.gitrepos}} 저장소가 포함될 수 있습니다. 

[YouTube ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://youtu.be/2SIPE1e7NJ4){: new_window} 또는 [{{site.data.keyword.contdelivery_short}} 시작하기](/docs/services/ContinuousDelivery/index.html)에서 도구 체인에 대해 자세히 알아볼 수 있습니다.
[![YouTube에 대한 외부 링크](images/CD_video.png)](https://youtu.be/2SIPE1e7NJ4){: new_window}


## 도구 체인 시작하기
{: #upgrade_next_steps}

1. 팀 구성원에게 도구 체인에 대한 액세스 권한을 부여하십시오. 
    - 각 팀 구성원은 유효한 {{site.data.keyword.Bluemix_notm}} 계정을 보유해야 합니다. 계정이 없는 팀 구성원은 [등록 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.ng.bluemix.net/registration){:new_window}이 필요합니다. 
    - 도구 체인 관리 페이지에서 조직 구성원에게 도구 체인에 액세스하는 권한을 부여하십시오. 기존 프로젝트 구성원은 업그레이드 프로세스의 일부로 도구 체인의 구성원으로 추가됩니다. 도구 체인의 액세스 제어에 대한 자세한 정보는 [액세스 관리![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](/docs/services/ContinuousDelivery/toolchains_using.html#managing_access){:new_window}를 참조하십시오.
    - 사용자가 도구 체인이 속한 조직의 구성원이 아니면 조직 관리 페이지에서 조직에 사용자를 추가하십시오.
      
    - 도구 체인에서 {{site.data.keyword.gitrepos}}을 사용하는 경우 유효한 Bluemix ID를 소유한 모든 JazzHub 프로젝트 구성원이 JazzHub 프로젝트에서와 동일한 권한과 함께 {{site.data.keyword.gitrepos}} 저장소에 추가됩니다. JazzHub 프로젝트에 유효한 Bluemix ID가 없는 구성원이 포함된 경우 해당 구성원은 Bluemix ID를 등록할 수 있습니다. 등록하면 저장소에 추가할 수 있습니다. 조직 관리에 대한 자세한 정보는 [조직 및 영역 관리![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](/docs/admin/orgs_spaces.html#orgsspacesusers){:new_window}를 참조하십시오.

2. {{site.data.keyword.gitrepos}}를 사용하는 경우 개인 액세스 토큰 또는 SSH 키를 사용하여 인증하십시오. SSH 키에 대한 자세한 정보는 [인증을 위한 개인 액세스 토큰 또는 SSH 키 작성](/docs/services/ContinuousDelivery/git_working.html#git_authentication)을 참조하십시오. https를 통해 외부 Git 클라이언트에서 인증하려면 다음 단계를 따르십시오.
    1. {{site.data.keyword.gitrepos}} 사용자 설정의 [액세스 토큰 페이지 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://git.ng.bluemix.net/profile/personal_access_tokens){:new_window}로 이동하십시오.
    2. **api**를 범위로 사용하는 개인 액세스 토큰을 작성하십시오.
    3. [계정 페이지![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://git.ng.bluemix.net/profile/account){:new_window}로 이동하고 {{site.data.keyword.gitrepos}}의 사용자 이름을 찾으십시오. 사용자 이름이 "사용자 이름 변경" 섹션에 나열되며 사용자가 작성한 개인 저장소 URL의 첫 번째 부분으로 표시됩니다.
    4. HTTPS를 통해 외부 Git 클라이언트에서 {{site.data.keyword.gitrepos}}를 인증하려면 사용자 이름과 개인 액세스 토큰을 사용하십시오.
    5. JazzHub Git 저장소의 로컬 저장소를 재사용하려면 저장소가 {{site.data.keyword.gitrepos}}의 새 저장소를 가리키게 지정하십시오. 터미널 쉘에서 JazzHub Git 저장소가 복제된 디렉토리로 변경하십시오. `git remote set-url` 명령을 입력하십시오. `git remote set-url origin https://git.ng.bluemix.net/<userid>/<name-of-new-repo>`

        **팁:** 어떤 원격 URL이 어떤 원격 이름으로 설정되었는지 확인하려면 `git remote -v` 명령을 사용하십시오. 기본 원격 이름은 `origin`입니다. 고급 설정이 있으면 명령의 형식은 다음과 같습니다. `git remote set-url<remote-name-that-uses-jazzhub-repo> https://git.ng.bluemix.net/<userid>/<name-of-new-repo>`

3. 선택사항: 프로젝트의 개발 성숙도, 팀의 사례 및 코드 베이스 품질을 탐색하려면 IBM Cloud {{site.data.keyword.DRA_short}}를 도구 체인에 추가하십시오. {{site.data.keyword.DRA_short}}에서는 개발자, 팀 및 배치 분석을 DevOps 프로젝트에 적용합니다. 자세한 정보는 [{{site.data.keyword.DRA_short}} 시작하기](/docs/services/DevOpsInsights/index.html)를 참조하십시오.


## 문제점 해결
{: #upgrade_troubleshoot}

프로젝트의 업그레이드와 관련된 문제점이 발생하면 [지원 포럼![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://developer.ibm.com/answers/questions/ask/?smartspace=devops-services){:new_window}을 참조하십시오. 포럼 게시물에 {{site.data.keyword.jazzhub_short}} 프로젝트와 {{site.data.keyword.contdelivery_short}} 도구 체인의 URL을 포함시키고 `devops-services` 태그로 게시물의 태그를 지정하십시오.


## 자주 묻는 질문(FAQ)
{: #upgrade_faq}

### 내 JazzHub 프로젝트는 영국 지역과 연관되어 있지만 내 도구 체인은 미국 남부 지역에 있습니다. 이런 경우 어떻게 작업하게 됩니까?
{: #faq_region}

hub.jazz.net의 프로젝트와 도구 체인은 모두 미국 남부 지역에서 호스팅됩니다. 다른 지역(예: 영국 지역)에 앱을 배치하도록 프로젝트가 구성된 경우, 도구 체인으로 업그레이드된 후에도 앱이 여전히 그 지역으로 배치됩니다. 따라서 데이터를 호스팅하고 있는 위치와 관련하여 아무 것도 바뀌지 않습니다. 미래에는 더 많은 지역에서 도구 체인을 사용할 수 있게 됩니다.

### 업그레이드 후 Track &amp; Plan의 내 작업 항목 및 대시보드에 무슨 일이 발생했습니까?
{: #faq_tp}

{{site.data.keyword.contdelivery_short}} 서비스는 {{site.data.keyword.gitrepos}}를 통해 문제 추적 기능을 제공하며, IBM에서 호스팅하며 GitLab Community Edition을 기반으로 합니다. {{site.data.keyword.contdelivery_short}}는 다른 계획 및 문제 추적 도구(예: GitHub Issues 및 JIRA)와 통합도 지원합니다. 

업그레이드 프로세스 중에 Track &amp; Plan 작업 항목을 Git Issues로 마이그레이션하도록 선택할 수 있습니다. GitHub Issues 및 {{site.data.keyword.gitrepos}}에서는 모두 계획용 문제 추적 및 kanban 보드를 제공합니다. Git Repos and Issue Tracking의 kanban 기능인 Issue Boards에 대한 자세히 알아보려면 [Issue board![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://git.ng.bluemix.net/help/user/project/issue_board.md){: new_window}를 참조하십시오. 

더 이상 사용되지 않는 JazzHub Track &amp; Plan과 같은 기능이 필요한 경우, 클라우드에서 새 IBM Track and Plan 서비스를 사용자별 월별 기준으로 선택된 국가에서 구매하는 것이 가능합니다. 이 클라우드 서비스를 사용하여 Rational Team Concert&trade; 기여자 라이센스와 동등한 전체 기능을 단일 테넌트 클라우드 등록으로 얻게 됩니다. 

이 새 IBM Track and Plan on Cloud 서비스는 더 이상 사용되지 않는 JazzHub Track &amp; Plan보다 훨씬 더 풍부한 기능을 제공하여 프로세스 사용자 정의, 프로젝트 계층구조, SAFe&reg; 및 많은 다른 신속한 하이브리드 방식, 단일 프로젝트 이상으로 성장하도록 하는 확장성을 지원합니다. 이는 최신 버전인 Rational Team Concert 6.0.3을 기반으로 하며 다음 60일 후에는 버전 6.0.4가 되는 반면에 JazzHub Track &amp; Plan을 Rational Team Concert 5.x를 기반으로 합니다. 추가 서비스를 통해 데이터 마이그레이션이 IBM Track and Plan on Cloud에 가능합니다. 자세한 정보는 Connected Products SaaS 영업 담당자인 [Tom Hollowell ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](mailto:trhollow@us.ibm.com){:new_window}에게 문의합니다. 

IBM Track and Plan on Cloud에 대한 정보가 필요하거나 온라인으로 구매하려면 [IBM Marketplace![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://www.ibm.com/us-en/marketplace/cloud-change-management){: new_window}를 방문하십시오. 

빌드 자동화 및 소스 코드 관리를 구매하려면 [Rational Team Concert on Cloud![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://www.ibm.com/us-en/marketplace/change-and-configuration-management/purchase#product-header-top){: new_window}가 옵션입니다.

### 업그레이드 후 내 코드 저장소에 무슨 일이 발생했습니까?
{: #faq_repo}

업그레이드 후에 새 Git 서비스를 이전 서비스와 비교할 수 있게 됩니다. JazzHub 프로젝트와 github.com을 사용한 경우 도구 체인이 같은 GitHub 저장소에 연결됩니다. JazzHub 프로젝트가 IBM Hosted Git를 사용한 경우, 해당 저장소의 컨텐츠가 {{site.data.keyword.contdelivery_short}}의 일부이며 IBM에서 호스팅하는 {{site.data.keyword.gitrepos}}의 새 저장소로 복제됩니다. 

업그레이드 프로세스에서 각 저장소 유형을 취급하는 방법에 대한 세부사항은 다음 표를 참조하십시오.

|프로젝트 저장소|프로젝트 유형|도구 체인 저장소|
|:----------|:------------------------------|:------------------|
|github.com|사설 또는 공용|{{site.data.keyword.Bluemix_notm}} Public과 동일한 github.com 저장소.|
|hub.jazz.net/git|사설 또는 공용|{{site.data.keyword.Bluemix_notm}} 퍼블릭이 있는 {{site.data.keyword.gitrepos}}의 새 개인용 또는 공용 저장소.|
|Jazz SCM|사설 또는 공용|{{site.data.keyword.Bluemix_notm}} 퍼블릭이 있는 {{site.data.keyword.gitrepos}}의 새 개인용 또는 공용 저장소.|
{: caption="표 1. 도구 체인 저장소에 맵핑된 프로젝트 저장소" caption-side="top"}


### 업그레이드 후 내 프로젝트의 빌드 정의에 무슨 일이 발생했습니까?
{: #faq_build}

Delivery Pipeline 대신에 Jazz를 사용해서 소스 코드를 빌드하는 경우, 빌드 정의를 도구 체인의 Delivery Pipeline으로 수동으로 마이그레이션해야 합니다. 

소스 저장소로 Jazz SCM을 사용하고 Delivery Pipeline을 사용하여 코드를 빌드하는 경우, Jazz SCM의 소스가 Git 저장소로 자동으로 이동됩니다. Delivery Pipeline 구성은 Jazz SCM의 소스 대신에 Git 저장소에서 소스를 이용하게 되는 것을 제외하고 동일하게 유지됩니다. 

### 도구 체인으로 업그레이드된 내 프로젝트에 대한 조직을 작성해야 했습니다. 내 신용카드가 청구됩니까?
{: #faq_charges}

[종량과금제 고객 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://www.ibm.com/cloud-computing/bluemix/pricing){: new_window}으로서 런타임, 서비스 또는 Bluemix 카탈로그에 나열된 무료 할당액을 초과하는 컴포넌트를 사용하는 경우에는 비용이 청구됩니다. 사용량 추정은 [가격 책정 시트![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.ng.bluemix.net/?direct=classic/&cm_mc_uid=49681106114614956310454&cm_mc_sid_50200000=1495641296&cm_mc_sid_52640000=1494981898#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet){: new_window}를 참조하십시오. Continuous Delivery에 대한 현재 가격 책정은 [Bluemix 카탈로그![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.bluemix.net/catalog/services/continuous-delivery){: new_window}를 참조하십시오.

IBM 직원인 경우, 내부 IBM 프로젝트는 개인 신용카드 대신에 부서에 청구할 수 있습니다. IBM 직원에 대한 무료 할당액을 초과하는 리소스를 사용해야 하는 경우 지원 티켓을 작성하십시오. 

### 내 도구 체인을 찾을 수 없거나 액세스할 수 없습니다. 어떻게 해야 합니까?
{: #faq_find}

도구 체인이 Bluemix 조직에서 호스팅됩니다. 업그레이드 프로세스는 JazzHub 프로젝트의 모든 구성원을 도구 체인에 추가합니다. 그러나 Bluemix 조직의 소유자가 조직에 사용자를 추가하지 않으면 사용자는 도구 체인을 볼 수 없습니다. 

도구 체인에 액세스하려면 Bluemix로 이동하여 메뉴 아이콘을 클릭하고 **서비스 &gt; DevOps**를 클릭하십시오. 도구 체인 페이지가 열립니다. 사용자가 미국 남부 지역에 있고 도구 체인이 포함된 조직에 속해 있는지 확인하십시오. 도구 체인이 도구 체인 페이지에 나열되지 않으면 [이 FAQ 항목](#faq_uk)을 참조하십시오.

### 내 프로젝트는 영국 지역과 연관되어 있습니다. 업그레이드 후, 내 동료는 도구 체인에 액세스할 수 없고 Bluemix의 도구 체인 페이지에서 내 도구 체인을 볼 수 없다는 오류 메시지가 표시됩니다. 무엇이 문제입니까?
{: #faq_uk}

**전체 질문:**

내 프로젝트는 프로젝트 설정에 따라 {{site.data.keyword.Bluemix_notm}} 영국 지역과 연관되어 있습니다. JazzHub의 개요 페이지로 이동하고 기어처럼 보이는 **설정** 아이콘을 클릭한 후 **옵션 &gt; 이를 Bluemix 프로젝트로 설정: 지역**을 클릭하여 내 프로젝트 설정을 확인했습니다. 미국에서 프로젝트를 도구 체인으로 업그레이드한 후 다음 문제가 발생합니다. 

   1. 미국 조직을 선택하는 경우 미국 남부 지역의 조직에는 영역이 없으며 영역 작성을 요구하는 프롬프트가 표시된다는 메시지를 보게 됩니다. 미국에서는 어떠한 작업도 수행하고 싶지 않습니다. 
   
   2. 동료 중 일부가 기존 JazzHub 프로젝트의 구성원으로 나열되었더라도 도구 체인에 액세스할 수 없습니다. 영국 지역에서 **도구 체인 보기**를 클릭하여 앱 개요 페이지에서 도구 체인 열기를 시도하는 경우 "액세스가 거부됨" 메시지가 표시됩니다. 
   
   3. 영국 지역에서 **도구 체인 보기**를 클릭하여 앱 개요 페이지에서 직접 도구 체인에 액세스할 수 있더라도 도구 체인 페이지([https://console.bluemix.net/devops/toolchains?env_id=ibm:yp:us-south ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.bluemix.net/devops/toolchains?env_id=ibm:yp:us-south){: new_window})에 나열된 도구 체인을 볼 수 없습니다. 도구 체인을 수정할 수 없다는 메시지 또는 도구 체인이 없으므로 작성해야 한다는 메시지가 표시됩니다.  

**답변:**

미국 이외의 {{site.data.keyword.Bluemix_notm}} 조직의 구성원이고 업그레이드 전에 사용자의 조직을 미국 남부 지역으로 명시적으로 확장하지 않은 경우 문제가 발생할 수 있습니다. 두 가지 방식으로 이를 확인할 수 있습니다. 

   - 도구 체인 URL을 열 때 {{site.data.keyword.Bluemix_notm}} 헤더를 확인하십시오. 조직의 이름을 알게 되고 영역이 표시되지 않을 가능성이 큽니다. 
   
   - 도구 체인의 개요 페이지에서 **관리**를 클릭하십시오. 액세스 제어 페이지에서 **조직 관리자** 링크를 클릭하십시오. 도구 체인이 포함된 조직이 기본 페이지에 나열됩니다. 

업그레이드 시, 미국 이외의 조직이 미국에 존재하지 않으므로 업그레이드 중에 액세스 권한이 있는 다른 조직을 검색하여 사용자를 위해 다른 조직을 선택했습니다. 

미국에서 해당 {{site.data.keyword.Bluemix_notm}} 조직으로 전환하는 경우 도구 체인을 찾을 수 있습니다. 동료를 해당 조직에 추가하는 경우 액세스 권한이 부여됩니다. 이 도구 체인은 미국 이외의 조직에 계속 배치될 수 있습니다. 유일한 문제점은 두 조직이 개별적이라는 것입니다. 이에 따라 두 조직에서 사용자 관리를 자동으로 수행할 수 없습니다. 

미국 이외의 조직과 일치하도록 도구 체인을 미국 조직에 배치하려면 다음 단계를 수행하십시오. 

   1. [https://console.bluemix.net ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.bluemix.net){: new_window}에 로그인하고 사용자가 속한 미국 이외의 지역 및 조직을 선택하십시오. 
   
   2. {{site.data.keyword.Bluemix_notm}} 헤더에서 미국 남부 지역으로 전환하십시오. 해당 지역에 영역 작성을 요구하는 프롬프트가 표시됩니다. 
   
   3. 미국 남부 지역에 영역을 작성하여 사용자의 조직을 해당 지역으로 확장하십시오.  
   
   4. 업그레이드 프로세스를 통해 작성된 도구 체인을 삭제하십시오.  
   
      **참고:** Git 저장소는 자동으로 삭제되지 않습니다. Git 저장소를 수동으로 삭제하거나 우선 이름을 바꾸려고 할 수 있습니다. Git 저장소를 이미 변경한 경우 나중에 사용하도록 이후의 도구 체인을 전환할 수 있습니다. 

   5. JazzHub 프로젝트로 돌아가십시오. 다음 번 업그레이드 시도 중에 자체적으로 재설정해야 합니다. 재설정하지 않으면 hub@jazz.net에 문의하여 프로젝트의 URL을 제공하십시오. 
   
   6. 업그레이드 프로세스를 다시 시작하고 미국 이외의 지역에서 사용자 조직의 이름과 일치하도록 미국에서 적절한 조직을 선택하십시오. 
   
   7. 이전 도구 체인 업그레이드 시도에서 Git 저장소를 유지하거나 이름을 바꾼 경우(단계 4 참조), 도구 체인에서 Git 카드를 재구성하여 이 Git 저장소 URL로 대신 지정할 수 있습니다. 변경사항이 파이프라인에서 자동으로 반영됩니다. 확인하려면 빌드 단계의 입력 탭을 검사하십시오. 
