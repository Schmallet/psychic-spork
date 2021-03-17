---
title: 查看企业帐户的订阅和使用情况
intro: '您可以查看企业帐户的当前订阅、许可证使用情况、发票、付款历史记录和其他结算信息。'
product: '{% data reusables.gated-features.enterprise-accounts %}'
permissions: '企业所有者和帐单管理员均可访问和管理企业帐户的所有帐单设置。'
redirect_from:
  - /github/setting-up-and-managing-your-enterprise-account/viewing-the-subscription-and-usage-for-your-enterprise-account
  - /articles/viewing-the-subscription-and-usage-for-your-enterprise-account
versions:
  free-pro-team: '*'
  enterprise-server: '*'
---

### 关于企业帐户的计费

企业帐户目前适用于通过发票付费的 {% data variables.product.prodname_enterprise %} 客户。 对与企业帐户关联的所有组织和 {% data variables.product.prodname_ghe_server %} 实例的结算将汇总为所有付费 {% data variables.product.prodname_dotcom_the_website %} 服务（包括组织中的付费许可、{% data variables.large_files.product_name_long %} 数据包和 {% data variables.product.prodname_marketplace %} 应用程序的订阅）的单一帐单费用。

{% if currentVersion == "free-pro-team@latest" %}{% data reusables.enterprise-accounts.billing-microsoft-ea-overview %} For more information, see "[Connecting an Azure subscription to your enterprise](/github/setting-up-and-managing-your-enterprise/connecting-an-azure-subscription-to-your-enterprise)."{% endif %}

有关管理帐单管理员的更多信息，请参阅“[邀请人员管理企业](/github/setting-up-and-managing-your-enterprise/inviting-people-to-manage-your-enterprise)”。

### 查看企业帐户的订阅和使用情况

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.license-tab %}
1. 在“User
{% if currentVersion == "free-pro-team@latest" %}Licenses{% else %}licenses{% endif %}（用户许可）”下，查看您的总许可数、已消耗许可数以及订阅到期日期。
  {% if currentVersion == "free-pro-team@latest" %}![License and subscription information in enterprise billing settings](/assets/images/help/business-accounts/billing-license-info.png){% else %}
  ![企业计费设置中的许可证和订阅信息](/assets/images/enterprise/enterprises/enterprise-server-billing-license-info.png){% endif %}
1. （可选）要查看许可使用详情或下载包含许可详情的 {% if currentVersion == "free-pro-team@latest" %}CSV{% elsif enterpriseServerVersions contains currentVersion %}JSON{% endif %} 文件{% if currentVersion == "free-pro-team@latest" %}，请在“User Licenses（用户许可）”的右侧{% endif %}，单击**查看{% if currentVersion == "free-pro-team@latest" %}详细信息{% elsif enterpriseServerVersions contains currentVersion %}用户{% endif %}**或{% if currentVersion == "free-pro-team@latest" %}{% octicon "download" aria-label="The download icon" %}{% elsif enterpriseServerVersions contains currentVersion %}**Export license usage（导出许可使用信息）**{% endif %}。{% if currentVersion == "free-pro-team@latest" %} !["View details" button and button with download icon to the right of "User Licenses"](/assets/images/help/business-accounts/billing-license-info-click-view-details-or-download.png){% endif %}