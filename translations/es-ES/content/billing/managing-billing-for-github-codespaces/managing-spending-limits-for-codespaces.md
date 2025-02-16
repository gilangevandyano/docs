---
title: Administrar los límites de gastos para los Codespaces
intro: Puedes configurar un límite de gastos para el uso de {% data variables.product.prodname_codespaces %}.
versions:
  fpt: '*'
  ghec: '*'
type: how_to
product: '{% data reusables.gated-features.codespaces %}'
topics:
- Codespaces
- Enterprise
- Organizations
- Spending limits
- User account
- Billing
shortTitle: Spending limits
ms.openlocfilehash: 340dae657304e5a2c9fb31d3a205e0b45f47a7b5
ms.sourcegitcommit: 22d665055b1bee7a5df630385e734e3a149fc720
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/13/2022
ms.locfileid: "145091695"
---
## <a name="about-spending-limits-for--data-variablesproductprodname_codespaces-"></a>Acerca de los límites de gastos para {% data variables.product.prodname_codespaces %}

{% data reusables.codespaces.codespaces-spending-limit-requirement %}

Una vez que hayas llegado a tu límite de gastos, tu organización o repositorio ya no podrán crear codespces nuevos y no podrán iniciar los existentes. Cualquier codespace existente que aún se esté ejecutando no se cerrará. Si no cambias el límite de gastos, no se tecobrará por la cantidad que exceda el límite.

Para más información sobre los precios de uso de {% data variables.product.prodname_codespaces %}, vea "[Acerca de la facturación de {% data variables.product.prodname_codespaces %}](/billing/managing-billing-for-github-codespaces/about-billing-for-codespaces)".

{% ifversion ghec %}
## <a name="using-your-azure-subscription"></a>Utilizar tu suscripción de Azure
Si compraste {% data variables.product.prodname_enterprise %} mediante un Acuerdo de Microsoft Enterprise, puedes conectar tu ID de Suscripción de Azure a tu cuenta empresarial para habilitar y pagar por el uso de {% data variables.product.prodname_codespaces %}. Para más información, vea "[Conexión de una suscripción de Azure a la empresa](/billing/managing-billing-for-your-github-account/connecting-an-azure-subscription-to-your-enterprise)".
{% endif %}

## <a name="managing-the-spending-limit-for--data-variablesproductprodname_codespaces--for-your-organization"></a>Administración del límite de gasto de {% data variables.product.prodname_codespaces %} para la organización

Los propietarios de las organizaciones y los administradores de facturación pueden administrar el límite de gasto de {% data variables.product.prodname_codespaces %} para una organización.

{% data reusables.organizations.billing-settings %} {% data reusables.dotcom_billing.manage-spending-limit %} {% data reusables.dotcom_billing.monthly-spending-limit-codespaces %} {% data reusables.dotcom_billing.update-spending-limit %}

{% ifversion ghec %}
## <a name="managing-the-spending-limit-for--data-variablesproductprodname_codespaces--for-your-enterprise-account"></a>Administración del límite de gasto de {% data variables.product.prodname_codespaces %} para la cuenta empresarial

Los propietarios de empresas y los administradores de facturación pueden administrar el límite de gasto para {% data variables.product.prodname_codespaces %} para una cuenta empresarial.

{% data reusables.enterprise-accounts.access-enterprise %} {% data reusables.enterprise-accounts.settings-tab %} {% data reusables.enterprise-accounts.billing-tab %}
1. Encima de "Uso mensual de {% data variables.product.prodname_codespaces %}", haga clic en **Spending Limit** (Límite de gasto).
  ![Pestaña Límite de gasto](/assets/images/help/settings/spending-limit-tab-enterprise.png) {% data reusables.dotcom_billing.monthly-spending-limit %} {% data reusables.dotcom_billing.update-spending-limit %} {% endif %}

## <a name="exporting-changes-when-you-have-reached-your-spending-limit"></a>Exportar cambios cuando llegaste a tu límite de gastos

{% data reusables.codespaces.exporting-changes %}
## <a name="managing-usage-and-spending-limit-email-notifications"></a>Administrar las notificaciones de uso y límite de gastos

Las notificaciones por correo electrónico se envían a los propietarios de las cuentas y gerentes de facturación cuando el límite de gastos llega a 50%, 75%, 90% y 100% del límite de gastos de tu cuenta. 

Puede deshabilitar estas notificaciones en cualquier momento si navega a la parte inferior de la página **Spending Limit** (Límite de gasto).

![Captura de pantalla de los ajustes de notificaciones de facturación por correo electrónico](/assets/images/help/billing/codespaces-spending-limit-notifications.png)

## <a name="further-reading"></a>Lecturas adicionales

- "[Restricción del acceso a los tipos de máquina](/codespaces/managing-codespaces-for-your-organization/restricting-access-to-machine-types)"
- "[Administración de la facturación de Codespaces en la organización](/codespaces/managing-codespaces-for-your-organization/managing-billing-for-codespaces-in-your-organization)"
