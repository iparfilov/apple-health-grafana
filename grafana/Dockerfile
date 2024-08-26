FROM grafana/grafana:11.1.0

ENV GF_SECURITY_ADMIN_USER=admin
ENV GF_SECURITY_ADMIN_PASSWORD=health
ENV GF_DASHBOARDS_DEFAULT_HOME_DASHBOARD_PATH=/etc/grafana/provisioning/dashboards/dashs/specific-metrics.json

# Enable embedding and anonymous access
ENV GF_AUTH_ANONYMOUS_ENABLED=true
ENV GF_SECURITY_ALLOW_EMBEDDING=true
ENV GF_AUTH_DISABLE_LOGIN_FORM=true

# Disable changing variables in the UI
ENV GF_VARIABLES_CUSTOM_ALLOW_UI_UPDATES=false

COPY provisioning/ /etc/grafana/provisioning/
