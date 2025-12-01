monitoring:
filebeat


application generique:
swagger
tracing
smtp_information
dlab_platform_informations
customer_cas_services
cas_services_configs
app_certificates
customer_certificates
contexts


vitamui:
=======
vitamui_assets
cas_server
iam_internal
security_internal
referential_internal
gateway
ui_identity
ui_identity_admin
ui_portal
ui_referential
ui_ingest
ui_archive_search
portal_categories

dlab:
=====

dlab_assets
docuware
common_asyncTasks
reporting_internal
reporting_batch
archive_internal
logistic_internal
logistic_external
flow_external
flow_internal

ui_archive
ui_flow
ui_flow_admin
ui_logistic
ui_reporting
ui_portal_xam
swagger_ui

qr_code
portal_categories
theme
scheduler
mailing
blocked_item


elca:
====
ui_wms
ui_wms_mobile
cas_services_configs


frontend:
========
frontend
frontend_user
frontend_group
frontend_certificates
frontend_ssl_global_certificate_enabled
frontend_configurations


# specific axone
axone_user_provisioning



# app specific a installer plus tard
bnpp_alert
bnpp_edi
provisioning_users
provisioning_client
bnpp_client
ui_provisioning


# specific consul
consul_data_center: "{{ current_env | regex_replace('-','_') }}"
consul_encrypt: "{{ vault_consul_secret }}"
consul_services: []
consul_recursors:  ["172.16.24.2", "10.197.3.16", "10.197.3.3"]



