# Comparing `tmp/nebari-2023.4.1a5.tar.gz` & `tmp/nebari-2023.5.1rc1.tar.gz`

## Comparing `nebari-2023.4.1a5.tar` & `nebari-2023.5.1rc1.tar`

### file list

```diff
@@ -1,501 +1,505 @@
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.cirun.yml
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.readthedocs.yml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/CONTRIBUTING.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/MANIFEST.in
--rw-r--r--   0        0        0    53015 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/RELEASE.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/flake.lock
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/flake.nix
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/noxfile.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/contributor.yaml
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/infracost.yml
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/kubernetes_test.yaml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/markdown.links.config.json
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/release.yaml
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/test.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/.gitignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/.gitmodules
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/README.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/conf.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/index.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/requirements.txt
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/_templates/announcement.html
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/_templates/layout.html
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/ext/substitute.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/output/.nojekyll
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/argo-workflows.md
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/awss3curl.md
--rw-r--r--   0        0        0     9441 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/backup.md
--rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/breaking-upgrade.md
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/clearml.md
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/cost.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/custom-helm-charts.md
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/faq.md
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/gpu.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/index.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/jupyterhub.md
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/keycloak.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/monitoring.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/preemptible-spot-instances.md
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/prefect.md
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/system_maintenance.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/traefik.md
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/troubleshooting.md
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/upgrade.md
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/architecture.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/changelog.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/contribution.md
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/index.md
--rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/keycloak.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/logo.md
--rw-r--r--   0        0        0    20441 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/minikube.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/release.md
--rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/testing.md
--rw-r--r--   0        0        0    64293 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/argo-server-landing-page.png
--rw-r--r--   0        0        0   221390 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudfare_update_screenshot.png
--rw-r--r--   0        0        0    17170 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_account_resources_scr.png
--rw-r--r--   0        0        0   108690 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_auth_1.png
--rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_permissions_2.1.1.png
--rw-r--r--   0        0        0    75331 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_summary.png
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_zone_resources.png
--rw-r--r--   0        0        0   277092 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/dev_postman_for_keycloak.png
--rw-r--r--   0        0        0   154819 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/grafana_manage_dashboards.png
--rw-r--r--   0        0        0    75305 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/grafana_networking_dashboard.png
--rw-r--r--   0        0        0    92141 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/grafana_node_cpu_usage.png
--rw-r--r--   0        0        0    94475 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/high_level_architecture.png
--rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/init_cli_output.png
--rw-r--r--   0        0        0    65086 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/k9s_UI.png
--rw-r--r--   0        0        0   156751 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_add_users.png
--rw-r--r--   0        0        0   161065 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_adduser.png
--rw-r--r--   0        0        0   131930 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_groups.png
--rw-r--r--   0        0        0   132035 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_master_login.png
--rw-r--r--   0        0        0    25405 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_new_group1.png
--rw-r--r--   0        0        0    94386 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_new_group2.png
--rw-r--r--   0        0        0   100928 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_new_group3.png
--rw-r--r--   0        0        0   317402 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_qhub_login.png
--rw-r--r--   0        0        0    97778 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_root_user_account_security.png
--rw-r--r--   0        0        0   157913 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_root_user_manage_account.png
--rw-r--r--   0        0        0   143079 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_root_user_update_password.png
--rw-r--r--   0        0        0   163577 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_user_password.png
--rw-r--r--   0        0        0    88640 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/labs_logo_white.png
--rw-r--r--   0        0        0    71430 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_api_token.png
--rw-r--r--   0        0        0    86104 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_api_token_generated.png
--rw-r--r--   0        0        0   185838 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_aws_architecture.png
--rw-r--r--   0        0        0   126188 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dashboard_notebook.png
--rw-r--r--   0        0        0    63407 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dashboard_resources.png
--rw-r--r--   0        0        0    56065 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dashboard_simple.png
--rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_options.png
--rw-r--r--   0        0        0    30695 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_start.png
--rw-r--r--   0        0        0   136024 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_do_architecture.png
--rw-r--r--   0        0        0   136194 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_gcp_architecture.png
--rw-r--r--   0        0        0    75740 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_kernel_selection.png
--rw-r--r--   0        0        0   102949 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_login_screen.png
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_logo.png
--rw-r--r--   0        0        0    44399 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_main_hub_page.png
--rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard.png
--rw-r--r--   0        0        0    61425 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard_filled_in.png
--rw-r--r--   0        0        0    45358 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_notebook.png
--rw-r--r--   0        0        0    69000 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_select_profile.png
--rw-r--r--   0        0        0    57906 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_server_start.png
--rw-r--r--   0        0        0   106710 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_vscode.png
--rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/quansight_logo_white.png
--rw-r--r--   0        0        0    20987 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/render_cli_output.png
--rw-r--r--   0        0        0    91557 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/tech_stack_diagram.png
--rw-r--r--   0        0        0    50197 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_env.png
--rw-r--r--   0        0        0    47961 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_instances.png
--rw-r--r--   0        0        0    57399 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_login_1.png
--rw-r--r--   0        0        0    53867 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_login_2.png
--rw-r--r--   0        0        0    25284 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_server_start.png
--rw-r--r--   0        0        0    38893 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/conda_icon.png
--rw-r--r--   0        0        0    26130 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/dask_icon.png
--rw-r--r--   0        0        0    62475 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/jupyter_hub_icon.png
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/nginx_icon.png
--rw-r--r--   0        0        0    34775 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/configuration.md
--rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/existing.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/index.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/installation.md
--rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/login.md
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/management.md
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/setup.md
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/usage.md
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/introduction/index.md
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/introduction/qhub-101.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/code_server.md
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/dashboard.md
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/dask_gateway.md
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/environments.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/experimental.md
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/faq.md
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/getting_started.md
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/idle_culler.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/index.md
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/ssh.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/training.md
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/troubleshooting.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/__main__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/_version.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/constants.py
--rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cost.py
--rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/deprecate.py
--rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/destroy.py
--rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/initialize.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/keycloak.py
--rw-r--r--   0        0        0    12982 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/render.py
--rw-r--r--   0        0        0    17548 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/schema.py
--rw-r--r--   0        0        0    14461 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/upgrade.py
--rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/utils.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/dev.py
--rw-r--r--   0        0        0    21893 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/init.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/keycloak.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/git.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/common.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/__init__.py
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/checks.py
--rw-r--r--   0        0        0    14391 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/input_vars.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/state_imports.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/tf_objects.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/main.tf
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/main.tf
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/locals.tf
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/main.tf
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/outputs.tf
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/providers.tf
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/versions.tf
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/existing/main.tf
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/outputs.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/provider.tf
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/main.tf
--rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/metallb.yaml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/outputs.tf
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/variables.tf
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/main.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/versions.tf
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
--rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/versions.tf
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/outputs.tf
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/versions.tf
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/argo-workflows.tf
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/clearml.tf
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/conda-store.tf
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/forward-auth.tf
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/kbatch.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/locals.tf
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/outputs.tf
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/prefect.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/providers.tf
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/versions.tf
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
--rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
--rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
--rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
--rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5139 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    15899 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/conda_store.json
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/jupyterhub.json
--rw-r--r--   0        0        0    52289 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/keycloak.json
--rw-r--r--   0        0        0    30301 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/traefik.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/versions.tf
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0    14303 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/conftest.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_cli.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_commons.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_dependencies.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_init.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_links.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_render.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_schema.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_upgrade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/notebooks/test-ipython-basic.ipynb
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/scripts/minikube-loadbalancer-ip.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/vale/styles/vocab.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/constants.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/LICENSE
--rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/README.md
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/pyproject.toml
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/PKG-INFO
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.cirun.yml
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.readthedocs.yml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/MANIFEST.in
+-rw-r--r--   0        0        0    56020 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/RELEASE.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/flake.lock
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/flake.nix
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/noxfile.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/contributor.yaml
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/infracost.yml
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/kubernetes_test.yaml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/markdown.links.config.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/.gitignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/.gitmodules
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/README.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/conf.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/index.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/requirements.txt
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/_templates/announcement.html
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/_templates/layout.html
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/ext/substitute.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/output/.nojekyll
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/argo-workflows.md
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/awss3curl.md
+-rw-r--r--   0        0        0     9441 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/backup.md
+-rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/breaking-upgrade.md
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/clearml.md
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/cost.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/custom-helm-charts.md
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/faq.md
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/gpu.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/index.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/jupyterhub.md
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/keycloak.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/monitoring.md
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/preemptible-spot-instances.md
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/prefect.md
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/system_maintenance.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/traefik.md
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/troubleshooting.md
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/admin_guide/upgrade.md
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/architecture.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/changelog.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/contribution.md
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/index.md
+-rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/keycloak.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/logo.md
+-rw-r--r--   0        0        0    20441 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/minikube.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/release.md
+-rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/dev_guide/testing.md
+-rw-r--r--   0        0        0    64293 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/argo-server-landing-page.png
+-rw-r--r--   0        0        0   102104 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/argo-workflows-user-tab.png
+-rw-r--r--   0        0        0   221390 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudfare_update_screenshot.png
+-rw-r--r--   0        0        0    17170 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_account_resources_scr.png
+-rw-r--r--   0        0        0   108690 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_auth_1.png
+-rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_permissions_2.1.1.png
+-rw-r--r--   0        0        0    75331 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_summary.png
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/cloudflare_zone_resources.png
+-rw-r--r--   0        0        0   277092 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/dev_postman_for_keycloak.png
+-rw-r--r--   0        0        0   154819 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/grafana_manage_dashboards.png
+-rw-r--r--   0        0        0    75305 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/grafana_networking_dashboard.png
+-rw-r--r--   0        0        0    92141 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/grafana_node_cpu_usage.png
+-rw-r--r--   0        0        0    94475 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/high_level_architecture.png
+-rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/init_cli_output.png
+-rw-r--r--   0        0        0    65086 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/k9s_UI.png
+-rw-r--r--   0        0        0   156751 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_add_users.png
+-rw-r--r--   0        0        0   161065 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_adduser.png
+-rw-r--r--   0        0        0   131930 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_groups.png
+-rw-r--r--   0        0        0   132035 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_master_login.png
+-rw-r--r--   0        0        0    25405 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_new_group1.png
+-rw-r--r--   0        0        0    94386 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_new_group2.png
+-rw-r--r--   0        0        0   100928 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_new_group3.png
+-rw-r--r--   0        0        0   317402 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_qhub_login.png
+-rw-r--r--   0        0        0    97778 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_account_security.png
+-rw-r--r--   0        0        0   157913 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_manage_account.png
+-rw-r--r--   0        0        0   143079 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_update_password.png
+-rw-r--r--   0        0        0   163577 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/keycloak_user_password.png
+-rw-r--r--   0        0        0    88640 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/labs_logo_white.png
+-rw-r--r--   0        0        0    71430 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_api_token.png
+-rw-r--r--   0        0        0    86104 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_api_token_generated.png
+-rw-r--r--   0        0        0   185838 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_aws_architecture.png
+-rw-r--r--   0        0        0   126188 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_notebook.png
+-rw-r--r--   0        0        0    63407 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_resources.png
+-rw-r--r--   0        0        0    56065 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_simple.png
+-rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dask_cluster_options.png
+-rw-r--r--   0        0        0    30695 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_dask_cluster_start.png
+-rw-r--r--   0        0        0   136024 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_do_architecture.png
+-rw-r--r--   0        0        0   136194 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_gcp_architecture.png
+-rw-r--r--   0        0        0    75740 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_kernel_selection.png
+-rw-r--r--   0        0        0   102949 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_login_screen.png
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_logo.png
+-rw-r--r--   0        0        0    44399 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_main_hub_page.png
+-rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_new_dashboard.png
+-rw-r--r--   0        0        0    61425 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_new_dashboard_filled_in.png
+-rw-r--r--   0        0        0    45358 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_notebook.png
+-rw-r--r--   0        0        0    69000 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_select_profile.png
+-rw-r--r--   0        0        0    57906 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_server_start.png
+-rw-r--r--   0        0        0   106710 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/qhub_vscode.png
+-rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/quansight_logo_white.png
+-rw-r--r--   0        0        0    20987 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/render_cli_output.png
+-rw-r--r--   0        0        0    91557 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/tech_stack_diagram.png
+-rw-r--r--   0        0        0    50197 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_env.png
+-rw-r--r--   0        0        0    47961 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_instances.png
+-rw-r--r--   0        0        0    57399 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_login_1.png
+-rw-r--r--   0        0        0    53867 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_login_2.png
+-rw-r--r--   0        0        0    25284 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/training_server_start.png
+-rw-r--r--   0        0        0    38893 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/conda_icon.png
+-rw-r--r--   0        0        0    26130 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/dask_icon.png
+-rw-r--r--   0        0        0    62475 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/jupyter_hub_icon.png
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/images/icons/nginx_icon.png
+-rw-r--r--   0        0        0    34775 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/configuration.md
+-rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/existing.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/index.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/installation.md
+-rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/login.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/management.md
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/setup.md
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/installation/usage.md
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/introduction/index.md
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/introduction/qhub-101.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/argo_workflows.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/code_server.md
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/dashboard.md
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/dask_gateway.md
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/environments.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/experimental.md
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/faq.md
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/getting_started.md
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/idle_culler.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/index.md
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/ssh.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/training.md
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/docs/source/user_guide/troubleshooting.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/__main__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/_version.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/constants.py
+-rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cost.py
+-rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/deprecate.py
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/destroy.py
+-rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/initialize.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/keycloak.py
+-rw-r--r--   0        0        0    12977 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/render.py
+-rw-r--r--   0        0        0    17590 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/schema.py
+-rw-r--r--   0        0        0    16652 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/upgrade.py
+-rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/utils.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/dev.py
+-rw-r--r--   0        0        0    22055 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/init.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/keycloak.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/git.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/__init__.py
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/checks.py
+-rw-r--r--   0        0        0    14771 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/input_vars.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/state_imports.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/main.tf
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/main.tf
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/locals.tf
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/main.tf
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/outputs.tf
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/main.tf
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/providers.tf
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/versions.tf
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/existing/main.tf
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/outputs.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/provider.tf
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/main.tf
+-rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/metallb.yaml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/outputs.tf
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/variables.tf
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/main.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/versions.tf
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
+-rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/versions.tf
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/outputs.tf
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/versions.tf
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0   358918 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/argo-workflows.tf
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/clearml.tf
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/conda-store.tf
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/dask_gateway.tf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/forward-auth.tf
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/kbatch.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/locals.tf
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/outputs.tf
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/prefect.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/providers.tf
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/versions.tf
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
+-rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
+-rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
+-rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10511 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     8942 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
+-rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
+-rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
+-rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/providers.tf
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/versions.tf
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0    14303 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_cli.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_commons.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_dependencies.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_init.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_links.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_render.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_schema.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/test_upgrade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/notebooks/test-ipython-basic.ipynb
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/scripts/minikube-loadbalancer-ip.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests/vale/styles/vocab.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/LICENSE
+-rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/README.md
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    11874 2020-02-02 00:00:00.000000 nebari-2023.5.1rc1/PKG-INFO
```

### Comparing `nebari-2023.4.1a5/.cirun.yml` & `nebari-2023.5.1rc1/.cirun.yml`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 runners:
   - name: run-k8s-tests
     # Cloud Provider: AWS
     cloud: aws
     # Instance Type has 4 vcpu, 16 GiB memory, Up to 5 Gbps Network Performance
     instance_type: t3a.xlarge
     # Custom AMI with docker/cypress/hub pre-installed
-    machine_image: ami-0cdc9ef51d44597ce
+    machine_image: ami-0a388df278199ff52
     # Region: Oregon
     region: us-west-2
     # Use Spot Instances for cost savings
     preemptible: false
     labels:
       - cirun-runner
```

### Comparing `nebari-2023.4.1a5/.pre-commit-config.yaml` & `nebari-2023.5.1rc1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Common tasks
 #
 # - Register git hooks: pre-commit install --install-hooks
 # - Run on all files:   pre-commit run --all-files
 #
 # These pre-commit hooks are run as CI.
 #
-# NOTE: if it can be avoided, add configs/args in pyproject.toml, setup.cfg or below instead of creating a new `.config.file`.
+# NOTE: if it can be avoided, add configs/args in pyproject.toml or below instead of creating a new `.config.file`.
 # https://pre-commit.ci/#configuration
 ci:
   autoupdate_schedule: monthly
   autofix_commit_msg: |
     [pre-commit.ci] Apply automatic pre-commit fixes
   # this does not work on pre-commit ci
   skip: [terraform_fmt]
@@ -33,35 +33,35 @@
         args: [--allow-multiple-documents]
       - id: check-toml
       # Lint: Checks that non-binary executables have a proper shebang.
       - id: check-executables-have-shebangs
         exclude: "^nebari/template/"
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         args:
           [
             "--builtin=rare,clear,informal,names",
             "--skip=_build,*/build/*,*/node_modules/*,nebari.egg-info,.nox,*.git,*.js,*.json,*.yaml,*.yml",
             "--ignore-words-list=AKS,aks",
             "--write",
           ]
         language: python
 
   # python
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: ["--line-length=88", "--exclude=/nebari/template/"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.254
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
@@ -69,15 +69,15 @@
         name: isort
         additional_dependencies: [toml]
         files: \.py$
         args: ["--profile", "black"]
 
   # terraform
   - repo: https://github.com/antonbabenko/pre-commit-terraform
-    rev: v1.77.1
+    rev: v1.78.0
     hooks:
       - id: terraform_fmt
         args:
           - --args=-write=true
 
   # markdown
   - repo: https://github.com/executablebooks/mdformat
```

### Comparing `nebari-2023.4.1a5/CODE_OF_CONDUCT.md` & `nebari-2023.5.1rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/CONTRIBUTING.md` & `nebari-2023.5.1rc1/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 > Our detailed contribution guidelines can be found [on Nebari's main documentation site][nebari-community].
 > Make sure to check the guidelines before you start contributing.
 
 ## Reporting issues
 
 When reporting issues please include as much detail as possible about your operating system, Nebari version, and dependencies version.
 Whenever possible, also include a brief, self-contained code example that demonstrates the problem.
-This [blog post by Matthew Rockling](https://matthewrocklin.com/blog/work/2018/02/28/minimal-bug-reports) is a good primer on how to craft minimal bug reports.
+This [blog post by Matthew Rocklin](https://matthewrocklin.com/blog/work/2018/02/28/minimal-bug-reports) is a good primer on how to craft minimal bug reports.
 
 - Use the [Nebari issue tracker][nebari-issues] for issues, bug reports, and feature requests for Nebari.
 - Use the [Nebari documentation issue tracker][nebari-docs-issues] for documentation-related improvements.
 - Read more about [best practices for issues creation](https://www.nebari.dev/docs/community/file-issues) in our community docs.
 
 <!-- Links -->
```

### Comparing `nebari-2023.4.1a5/RELEASE.md` & `nebari-2023.5.1rc1/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,55 @@
 If you want to update the release notes, open a PR against nebari-dev/nebari.
 This file is copied to nebari-dev/nebari-docs using a GitHub Action. -->
 
 ---
 
 ## Upcoming Release
 
+## Release 2023.4.1 - April 12, 2023
+
+> NOTE: Nebari requires Kubernetes version 1.23 and Digital Ocean now requires new clusters to run Kubernetes version 1.24. This means that if you are currently running on Digital Ocean, you should be fine but deploying on a new cluster on Digital Ocean is not possible until we upgrade Kubernetes version (see [issue 1622](https://github.com/nebari-dev/nebari/issues/1622) for more details).
+
+
 ### Feature changes and enhancements
 
+* Upgrades and improvements to conda-store including a new user-interface and greater administrator capabilities.
+* Idle-culler settings can now be configured directly from the `nebari-config.yaml`.
+
+
+### What's Changed
+* PR: Raise timeout for jupyter session by @ppwadhwa in https://github.com/nebari-dev/nebari/pull/1646
+* PR lower dashboard launch timeout by @ppwadhwa in https://github.com/nebari-dev/nebari/pull/1647
+* PR: Update dashboard environment by @ppwadhwa in https://github.com/nebari-dev/nebari/pull/1655
+* Fix doc link in README.md by @tkoyama010 in https://github.com/nebari-dev/nebari/pull/1660
+* PR: Update dask environment by @ppwadhwa in https://github.com/nebari-dev/nebari/pull/1654
+* Feature remove jupyterlab news by @costrouc in https://github.com/nebari-dev/nebari/pull/1641
+* [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/nebari-dev/nebari/pull/1644
+* Feat GitHub actions before_script and after_script steps by @costrouc in https://github.com/nebari-dev/nebari/pull/1672
+* Remove examples folder by @ppwadhwa in https://github.com/nebari-dev/nebari/pull/1664
+* Fix GH action typos by @kcpevey in https://github.com/nebari-dev/nebari/pull/1677
+* Github Actions CI needs id-token write permissions by @costrouc in https://github.com/nebari-dev/nebari/pull/1682
+* Update AWS force destroy script, include lingering volumes by @iameskild in https://github.com/nebari-dev/nebari/pull/1681
+* [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/nebari-dev/nebari/pull/1673
+* Make idle culler settings configurable from the `nebari-config.yaml` by @iameskild in https://github.com/nebari-dev/nebari/pull/1689
+* Update pyproject dependencies and add test to ensure it builds on conda-forge by @iameskild in https://github.com/nebari-dev/nebari/pull/1662
+* Retrieve secrets from Vault, fix test-provider CI by @iameskild in https://github.com/nebari-dev/nebari/pull/1676
+* Pull PyPI secrets from Vault by @iameskild in https://github.com/nebari-dev/nebari/pull/1696
+* Adding newest conda-store 0.4.14 along with superadmin credentials by @costrouc in https://github.com/nebari-dev/nebari/pull/1701
+* Update release notes for 2023.4.1 by @iameskild in https://github.com/nebari-dev/nebari/pull/1722
+
+### New Contributors
+* @ppwadhwa made their first contribution in https://github.com/nebari-dev/nebari/pull/1646
+* @tkoyama010 made their first contribution in https://github.com/nebari-dev/nebari/pull/1660
+
+**Full Changelog**: https://github.com/nebari-dev/nebari/compare/2023.1.1...2023.4.1
+
 ## Release 2023.1.1 - January 30, 2023
 
-## What's Changed
+### What's Changed
 * 🔄 Synced file(s) with nebari-dev/.github by @nebari-sensei in https://github.com/nebari-dev/nebari/pull/1588
 * Make conda-store file system read-only by default by @alimanfoo in https://github.com/nebari-dev/nebari/pull/1595
 * ENH - Switch to ruff and pre-commit.ci by @trallard in https://github.com/nebari-dev/nebari/pull/1602
 * Migrate to hatch by @iameskild in https://github.com/nebari-dev/nebari/pull/1545
 * Add check_repository_cred function to CLI by @iameskild in https://github.com/nebari-dev/nebari/pull/1605
 * Adding jupyterlab-conda-store extension support to Nebari by @costrouc in https://github.com/nebari-dev/nebari/pull/1564
 * [pre-commit.ci] pre-commit autoupdate by @pre-commit-ci in https://github.com/nebari-dev/nebari/pull/1613
@@ -30,15 +66,15 @@
 * Add option for AWS node-groups to run in a single subnet/AZ by @iameskild in https://github.com/nebari-dev/nebari/pull/1428
 * Add export-users to keycloak CLI command, add dev CLI command by @iameskild in https://github.com/nebari-dev/nebari/pull/1610
 * Unpin packages in default dashboard env by @iameskild in https://github.com/nebari-dev/pull/1628
 * Add release notes for 2023.1.1 by @iameskild in https://github.com/nebari-dev/nebari/pull/1629
 * Set GKE release_channel to unspecified to prevent auto k8s updates by @iameskild in https://github.com/nebari-dev/nebari/pull/1630
 * Update default nebari-dask, nebari image tags by @iameskild in https://github.com/nebari-dev/nebari/pull/1636
 
-## New Contributors
+### New Contributors
 * @pre-commit-ci made their first contribution in https://github.com/nebari-dev/nebari/pull/1613
 
 
 ## Release 2022.11.1 - December 1, 2022
 
 ### What's Changed
```

### Comparing `nebari-2023.4.1a5/flake.lock` & `nebari-2023.5.1rc1/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/flake.nix` & `nebari-2023.5.1rc1/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2023.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2023.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/workflows/infracost.yml` & `nebari-2023.5.1rc1/.github/workflows/infracost.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/workflows/kubernetes_test.yaml` & `nebari-2023.5.1rc1/.github/workflows/kubernetes_test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,30 @@
     paths:
       - ".github/workflows/kubernetes_test.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
       - "nebari/**"
-      - "setup.cfg"
       - "pyproject.toml"
+      - "pytest.ini"
   push:
     branches:
       - main
       - develop
       - release/\d{4}.\d{1,2}.\d{1,2}
     paths:
       - ".github/workflows/kubernetes_test.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
       - "nebari/**"
-      - "setup.cfg"
       - "pyproject.toml"
+      - "pytest.ini"
   workflow_call:
     inputs:
       pr_number:
         required: true
         type: string
 
 jobs:
@@ -64,15 +64,15 @@
         env:
           CONDA: /home/runnerx/miniconda3
         with:
           python-version: 3.8
           miniconda-version: "latest"
       - name: Install Nebari
         run: |
-          conda install -c anaconda pip
+          conda install --quiet --yes -c anaconda pip
           pip install .[dev]
       - name: Download and Install Kubectl
         run: |
           mkdir -p bin
           pushd bin
 
           curl -LO https://storage.googleapis.com/kubernetes-release/release/v1.19.0/bin/linux/amd64/kubectl
@@ -168,14 +168,15 @@
           export KEYCLOAK_PASSWORD=${CYPRESS_EXAMPLE_USER_PASSWORD}
           pytest tests_deployment/ -v -s
 
       - name: JupyterHub Notebook Tests
         # run jhub-client after pytest since jhubctl can cleanup
         # the running server
         run: |
+          sleep 60
           export JUPYTERHUB_USERNAME=${CYPRESS_EXAMPLE_USER_NAME}
           export JUPYTERHUB_PASSWORD=${CYPRESS_EXAMPLE_USER_PASSWORD}
           jhubctl --verbose run --hub=https://github-actions.nebari.dev \
                                 --auth-type=keycloak \
                                 --validate --no-verify-ssl \
                                 --kernel python3 \
                                 --stop-server \
```

### Comparing `nebari-2023.4.1a5/.github/workflows/markdown.links.config.json` & `nebari-2023.5.1rc1/.github/workflows/markdown.links.config.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.github/workflows/release-notes-sync.yaml` & `nebari-2023.5.1rc1/.github/workflows/release-notes-sync.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -10,12 +10,12 @@
     runs-on: ubuntu-latest
     steps:
       - name: Checkout Repository
         uses: actions/checkout@master
       - name: Run Release File Sync ♻️
         uses: BetaHuhn/repo-file-sync-action@v1
         with:
-          GH_PAT: ${{ secrets.GITHUB_TOKEN }}
+          GH_PAT: ${{ secrets.NEBARI_SENSEI_API_DOCS_PR_OPENER }}
           CONFIG_PATH: .github/release-notes-sync-config.yaml
           COMMIT_BODY: "MAINT - Sync release notes :robot:"
           PR_LABELS: |
             type: file sync ♻️
```

### Comparing `nebari-2023.4.1a5/.github/workflows/release.yaml` & `nebari-2023.5.1rc1/.github/workflows/release.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
       - name: Build source and binary
         run: python -m build --sdist --wheel .
 
       - name: Retrieve secret from Vault
         uses: hashicorp/vault-action@v2.5.0
         with:
           method: jwt
-          url: "https://quansight-public-vault-fe415d04.c219cf75.z1.hashicorp.cloud:8200"
+          url: "https://quansight-vault-public-vault-b2379fa7.d415e30e.z1.hashicorp.cloud:8200"
           namespace: "admin/quansight"
           role: "repository-nebari-dev-nebari-role"
           secrets: |
             kv/data/repository/nebari-dev/nebari/shared_secrets PYPI_USERNAME | PYPI_USERNAME;
             kv/data/repository/nebari-dev/nebari/shared_secrets PYPI_PASSWORD | PYPI_PASSWORD;
 
       - name: Publish package
```

### Comparing `nebari-2023.4.1a5/.github/workflows/run-precommit.yaml` & `nebari-2023.5.1rc1/.github/workflows/run-precommit.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -15,15 +15,11 @@
     defaults:
       run:
         shell: bash -l {0}
     steps:
       - name: Checkout repository 🔔
         uses: actions/checkout@v3
 
-      # https://github.com/pre-commit/action to enable cache
-      - uses: pre-commit/action@v3.0.0
-
-      - name: Install pre-commit 📦
-        run: pip install pre-commit
-
       - name: Run terraform pre-commit ⚡️
-        run: pre-commit run terraform_fmt
+        uses: pre-commit/action@v3.0.0
+        with:
+          extra_args: --all-files terraform_fmt
```

### Comparing `nebari-2023.4.1a5/.github/workflows/test-provider.yaml` & `nebari-2023.5.1rc1/.github/workflows/test-provider.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,27 @@
     paths:
       - ".github/workflows/test-provider.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
       - "nebari/**"
-      - "setup.cfg"
       - "pyproject.toml"
   push:
     branches:
       - main
       - develop
       - release/\d{4}.\d{1,2}.\d{1,2}
     paths:
       - ".github/workflows/test-provider.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
       - "nebari/**"
-      - "setup.cfg"
       - "pyproject.toml"
   workflow_call:
     inputs:
       pr_number:
         required: true
         type: string
 
@@ -41,15 +39,15 @@
       contents: read
       pull-requests: write
     strategy:
       matrix:
         provider:
           - aws
           - azure
-          # - do
+          - do
           - gcp
           - local
           - existing
         cicd:
           - none
           - github-actions
           - gitlab-ci
@@ -68,26 +66,26 @@
         with:
           python-version: 3.8
 
       - name: Retrieve secret from Vault
         uses: hashicorp/vault-action@v2.5.0
         with:
           method: jwt
-          url: "https://quansight-public-vault-fe415d04.c219cf75.z1.hashicorp.cloud:8200"
+          url: "https://quansight-vault-public-vault-b2379fa7.d415e30e.z1.hashicorp.cloud:8200"
           namespace: "admin/quansight"
           role: "repository-nebari-dev-nebari-role"
           secrets: |
             kv/data/repository/nebari-dev/nebari/amazon_web_services/nebari-dev-ci role_name | AWS_ROLE_ARN;
             kv/data/repository/nebari-dev/nebari/google_cloud_platform/nebari-dev-ci/github-nebari-dev-repo-ci project_id | PROJECT_ID;
             kv/data/repository/nebari-dev/nebari/google_cloud_platform/nebari-dev-ci/github-nebari-dev-repo-ci workload_identity_provider | GCP_WORKFLOW_PROVIDER;
             kv/data/repository/nebari-dev/nebari/google_cloud_platform/nebari-dev-ci/github-nebari-dev-repo-ci service_account_name | GCP_SERVICE_ACCOUNT;
             kv/data/repository/nebari-dev/nebari/azure/nebari-dev-ci/github-nebari-dev-repo-ci client_id | ARM_CLIENT_ID;
             kv/data/repository/nebari-dev/nebari/azure/nebari-dev-ci/github-nebari-dev-repo-ci tenant_id | ARM_TENANT_ID;
             kv/data/repository/nebari-dev/nebari/azure/nebari-dev-ci/github-nebari-dev-repo-ci subscription_id | ARM_SUBSCRIPTION_ID;
-          # kv/data/repository/nebari-dev/nebari/shared_secrets DIGITALOCEAN_TOKEN | DIGITALOCEAN_TOKEN;
+            kv/data/repository/nebari-dev/nebari/shared_secrets DIGITALOCEAN_TOKEN | DIGITALOCEAN_TOKEN;
 
       - name: 'Authenticate to GCP'
         if: ${{ matrix.provider == 'gcp' }}
         uses: 'google-github-actions/auth@v1'
         with:
           token_format: access_token
           create_credentials_file: 'true'
@@ -113,14 +111,15 @@
         with:
           client-id: ${{ env.ARM_CLIENT_ID }}
           tenant-id: ${{ env.ARM_TENANT_ID }}
           subscription-id: ${{ env.ARM_SUBSCRIPTION_ID }}
 
       - name: Install Nebari
         run: |
+          pip install --upgrade pip
           pip install .[dev]
 
       - name: Nebari Initialize
         run: |
           nebari init "${{ matrix.provider }}" --project "TestProvider" --domain "${{ matrix.provider }}.nebari.dev" --auth-provider github --disable-prompt --ci-provider ${{ matrix.cicd }}
           cat "nebari-config.yaml"
```

### Comparing `nebari-2023.4.1a5/.github/workflows/test.yaml` & `nebari-2023.5.1rc1/.github/workflows/test.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,30 @@
     paths:
       - ".github/workflows/test.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
       - "nebari/**"
-      - "setup.cfg"
       - "pyproject.toml"
+      - "pytest.ini"
   push:
     branches:
       - main
       - develop
       - release/\d{4}.\d{1,2}.\d{1,2}
     paths:
       - ".github/workflows/test.yaml"
       - "tests/**"
       - "tests_deployment/**"
       - "tests_e2e/**"
       - "scripts/**"
       - "nebari/**"
-      - "setup.cfg"
       - "pyproject.toml"
+      - "pytest.ini"
 
 jobs:
   test-general:
     name: "Pytest"
     runs-on: ubuntu-latest
     strategy:
       matrix:
@@ -47,12 +47,12 @@
         with:
           python-version: ${{ matrix.python-version }}
           channel-priority: strict
           channels: conda-forge
       - name: Install Nebari
         run: |
           pip install .[dev]
-          conda install conda-build -y
+          conda install --quiet --yes conda-build
       - name: Test Nebari
         run: |
           pytest --version
           pytest --ignore=tests_deployment
```

### Comparing `nebari-2023.4.1a5/docs/.gitignore` & `nebari-2023.5.1rc1/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/conf.py` & `nebari-2023.5.1rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/index.md` & `nebari-2023.5.1rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/ext/substitute.py` & `nebari-2023.5.1rc1/docs/ext/substitute.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/argo-workflows.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/argo-workflows.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 # Argo Workflows
 
 Argo Workflows is an open source container-native workflow engine for orchestrating parallel jobs on Kubernetes. Argo
-workflows comes enabled by default with Qhub deployments.
+workflows comes enabled by default with Nebari deployments.
 
 ## Accessing Argo Server
 
-If Argo Workflows is enabled, users can access argo workflows server at: `your-qhub-domain.com/argo`. Log in via
+If Argo Workflows is enabled, users can access argo workflows server at: `your-nebari-domain.com/argo`. Log in via
 Keycloak with your usual credentials.
 
-Refer to the [Argo documentation](https://argoproj.github.io/argo-workflows/) for further details on Argo Workflows.
-
-## Submitting a workflow via Argo Server
-
-You can submit a workflow by clicking "SUBMIT NEW WORKFLOW" on the landing page.
-
-![See Argo Server Landing Page](../images/argo-server-landing-page.png)
-
 ## Overrides of Argo Workflows Helm Chart values
 
-Argo Workflows is deployed using Argo Workflows Helm Chart version 0.13.1. The values.yaml for the helm chart can be
-overridden as needed via the overrides flag. The default values file can be found
-[here](https://github.com/argoproj/argo-helm/blob/argo-workflows-0.13.1/charts/argo-workflows/values.yaml). For example,
+Argo Workflows is deployed using the Argo Workflows Helm Chart. The values.yaml for the helm chart can be overridden as
+needed via the overrides flag. The default values file can be found
+[here](https://github.com/argoproj/argo-helm/blob/argo-workflows-0.22.9/charts/argo-workflows/values.yaml). For example,
 the following could be done to add additional environment variables to the controller container.
 
 ```yaml
 argo_workflows:
   enabled: true
   overrides:
     controller:
       extraEnv:
         - name: foo
           value: bar
 ```
 
 ## Disabling Argo Workflows
 
-To turn off the cluster monitoring on QHub deployments, simply turn off the feature flag within your `qhub-config.yaml`
-file. For example:
+To turn off the cluster monitoring on Nebari deployments, simply turn off the feature flag within your
+`nebari-config.yaml` file. For example:
 
 ```yaml
 argo_workflows:
   enabled: false
 ```
+
+Refer to the [Argo documentation](https://argoproj.github.io/argo-workflows/) for further details on Argo Workflows.
```

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/awss3curl.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/awss3curl.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/backup.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/backup.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/breaking-upgrade.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/breaking-upgrade.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/clearml.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/clearml.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/cost.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/cost.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/custom-helm-charts.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/custom-helm-charts.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/faq.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/faq.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/gpu.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/gpu.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/jupyterhub.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/jupyterhub.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/keycloak.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/keycloak.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/monitoring.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/monitoring.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/preemptible-spot-instances.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/preemptible-spot-instances.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/prefect.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/prefect.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/system_maintenance.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/system_maintenance.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/traefik.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/traefik.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/troubleshooting.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/admin_guide/upgrade.md` & `nebari-2023.5.1rc1/docs/source/admin_guide/upgrade.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/dev_guide/architecture.md` & `nebari-2023.5.1rc1/docs/source/dev_guide/architecture.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/dev_guide/contribution.md` & `nebari-2023.5.1rc1/docs/source/dev_guide/contribution.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/dev_guide/keycloak.md` & `nebari-2023.5.1rc1/docs/source/dev_guide/keycloak.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/dev_guide/minikube.md` & `nebari-2023.5.1rc1/docs/source/dev_guide/minikube.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/dev_guide/release.md` & `nebari-2023.5.1rc1/docs/source/dev_guide/release.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/dev_guide/testing.md` & `nebari-2023.5.1rc1/docs/source/dev_guide/testing.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/argo-server-landing-page.png` & `nebari-2023.5.1rc1/docs/source/images/argo-server-landing-page.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/cloudfare_update_screenshot.png` & `nebari-2023.5.1rc1/docs/source/images/cloudfare_update_screenshot.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/cloudflare_account_resources_scr.png` & `nebari-2023.5.1rc1/docs/source/images/cloudflare_account_resources_scr.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/cloudflare_auth_1.png` & `nebari-2023.5.1rc1/docs/source/images/cloudflare_auth_1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/cloudflare_permissions_2.1.1.png` & `nebari-2023.5.1rc1/docs/source/images/cloudflare_permissions_2.1.1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/cloudflare_summary.png` & `nebari-2023.5.1rc1/docs/source/images/cloudflare_summary.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/cloudflare_zone_resources.png` & `nebari-2023.5.1rc1/docs/source/images/cloudflare_zone_resources.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/dev_postman_for_keycloak.png` & `nebari-2023.5.1rc1/docs/source/images/dev_postman_for_keycloak.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/grafana_manage_dashboards.png` & `nebari-2023.5.1rc1/docs/source/images/grafana_manage_dashboards.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/grafana_networking_dashboard.png` & `nebari-2023.5.1rc1/docs/source/images/grafana_networking_dashboard.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/grafana_node_cpu_usage.png` & `nebari-2023.5.1rc1/docs/source/images/grafana_node_cpu_usage.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/high_level_architecture.png` & `nebari-2023.5.1rc1/docs/source/images/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/init_cli_output.png` & `nebari-2023.5.1rc1/docs/source/images/init_cli_output.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/k9s_UI.png` & `nebari-2023.5.1rc1/docs/source/images/k9s_UI.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_add_users.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_add_users.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_adduser.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_adduser.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_groups.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_groups.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_master_login.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_master_login.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_new_group1.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_new_group1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_new_group2.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_new_group2.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_new_group3.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_new_group3.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_qhub_login.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_qhub_login.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_root_user_account_security.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_account_security.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_root_user_manage_account.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_manage_account.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_root_user_update_password.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_root_user_update_password.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/keycloak_user_password.png` & `nebari-2023.5.1rc1/docs/source/images/keycloak_user_password.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/labs_logo_white.png` & `nebari-2023.5.1rc1/docs/source/images/labs_logo_white.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_api_token.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_api_token.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_api_token_generated.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_api_token_generated.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_aws_architecture.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_aws_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_dashboard_notebook.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_notebook.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_dashboard_resources.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_resources.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_dashboard_simple.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_dashboard_simple.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_options.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_dask_cluster_options.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_start.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_dask_cluster_start.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_do_architecture.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_do_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_gcp_architecture.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_gcp_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_kernel_selection.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_kernel_selection.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_login_screen.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_login_screen.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_logo.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_logo.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_main_hub_page.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_main_hub_page.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_new_dashboard.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard_filled_in.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_new_dashboard_filled_in.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_notebook.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_notebook.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_select_profile.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_select_profile.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_server_start.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_server_start.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/qhub_vscode.png` & `nebari-2023.5.1rc1/docs/source/images/qhub_vscode.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/quansight_logo_white.png` & `nebari-2023.5.1rc1/docs/source/images/quansight_logo_white.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/render_cli_output.png` & `nebari-2023.5.1rc1/docs/source/images/render_cli_output.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/tech_stack_diagram.png` & `nebari-2023.5.1rc1/docs/source/images/tech_stack_diagram.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/training_env.png` & `nebari-2023.5.1rc1/docs/source/images/training_env.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/training_instances.png` & `nebari-2023.5.1rc1/docs/source/images/training_instances.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/training_login_1.png` & `nebari-2023.5.1rc1/docs/source/images/training_login_1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/training_login_2.png` & `nebari-2023.5.1rc1/docs/source/images/training_login_2.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/training_server_start.png` & `nebari-2023.5.1rc1/docs/source/images/training_server_start.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/icons/conda_icon.png` & `nebari-2023.5.1rc1/docs/source/images/icons/conda_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/icons/dask_icon.png` & `nebari-2023.5.1rc1/docs/source/images/icons/dask_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/icons/jupyter_hub_icon.png` & `nebari-2023.5.1rc1/docs/source/images/icons/jupyter_hub_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/images/icons/nginx_icon.png` & `nebari-2023.5.1rc1/docs/source/images/icons/nginx_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/installation/configuration.md` & `nebari-2023.5.1rc1/docs/source/installation/configuration.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/installation/existing.md` & `nebari-2023.5.1rc1/docs/source/installation/existing.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/installation/installation.md` & `nebari-2023.5.1rc1/docs/source/installation/installation.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/installation/login.md` & `nebari-2023.5.1rc1/docs/source/installation/login.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/installation/management.md` & `nebari-2023.5.1rc1/docs/source/installation/management.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/installation/setup.md` & `nebari-2023.5.1rc1/docs/source/installation/setup.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/installation/usage.md` & `nebari-2023.5.1rc1/docs/source/installation/usage.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/introduction/index.md` & `nebari-2023.5.1rc1/docs/source/introduction/index.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/introduction/qhub-101.md` & `nebari-2023.5.1rc1/docs/source/introduction/qhub-101.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/code_server.md` & `nebari-2023.5.1rc1/docs/source/user_guide/code_server.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/dashboard.md` & `nebari-2023.5.1rc1/docs/source/user_guide/dashboard.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/dask_gateway.md` & `nebari-2023.5.1rc1/docs/source/user_guide/dask_gateway.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/environments.md` & `nebari-2023.5.1rc1/docs/source/user_guide/environments.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/faq.md` & `nebari-2023.5.1rc1/docs/source/user_guide/faq.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/getting_started.md` & `nebari-2023.5.1rc1/docs/source/user_guide/getting_started.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/idle_culler.md` & `nebari-2023.5.1rc1/docs/source/user_guide/idle_culler.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/ssh.md` & `nebari-2023.5.1rc1/docs/source/user_guide/ssh.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/training.md` & `nebari-2023.5.1rc1/docs/source/user_guide/training.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/docs/source/user_guide/troubleshooting.md` & `nebari-2023.5.1rc1/docs/source/user_guide/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/cost.py` & `nebari-2023.5.1rc1/nebari/cost.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/deploy.py` & `nebari-2023.5.1rc1/nebari/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/destroy.py` & `nebari-2023.5.1rc1/nebari/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/initialize.py` & `nebari-2023.5.1rc1/nebari/initialize.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/keycloak.py` & `nebari-2023.5.1rc1/nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/render.py` & `nebari-2023.5.1rc1/nebari/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 from typing import Dict, List
 
 import yaml
 from rich import print
 from rich.table import Table
 from ruamel.yaml import YAML
 
+import nebari
 from nebari.deprecate import DEPRECATED_FILE_PATHS
 from nebari.provider.cicd.github import gen_nebari_linter, gen_nebari_ops
 from nebari.provider.cicd.gitlab import gen_gitlab_ci
 from nebari.stages import tf_objects
 
 
 def render_template(output_directory, config_filename, force=False, dry_run=False):
     # get directory for nebari templates
-    import nebari
-
     template_directory = pathlib.Path(nebari.__file__).parent / "template"
 
     # would be nice to remove assumption that input directory
     # is in local filesystem and a directory
     template_directory = pathlib.Path(template_directory)
     if not template_directory.is_dir():
         raise ValueError(f"template directory={template_directory} is not a directory")
```

### Comparing `nebari-2023.4.1a5/nebari/schema.py` & `nebari-2023.5.1rc1/nebari/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,15 @@
 
 class GoogleCloudPlatformProvider(Base):
     project: str
     region: str
     zone: typing.Optional[str]  # No longer used
     availability_zones: typing.Optional[typing.List[str]]  # Genuinely optional
     kubernetes_version: str
+    release_channel: typing.Optional[str]
     node_groups: typing.Dict[str, NodeGroup]
     terraform_overrides: typing.Any
 
 
 class AzureProvider(Base):
     region: str
     kubernetes_version: str
```

### Comparing `nebari-2023.4.1a5/nebari/upgrade.py` & `nebari-2023.5.1rc1/nebari/upgrade.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,40 +4,46 @@
 import re
 import secrets
 import string
 from abc import ABC
 
 import rich
 from pydantic.error_wrappers import ValidationError
+from rich.prompt import Prompt
 
 from .schema import is_version_accepted, verify
 from .utils import backup_config_file, load_yaml, yaml
 from .version import __version__, rounded_ver_parse
 
 logger = logging.getLogger(__name__)
 
 
 def do_upgrade(config_filename, attempt_fixes=False):
     config = load_yaml(config_filename)
+    if config.get("qhub_version"):
+        rich.print(
+            f"Your config file [purple]{config_filename}[/purple] uses the deprecated qhub_version key.  Please change qhub_version to nebari_version and re-run the upgrade command."
+        )
+        return
 
     try:
         verify(config)
         rich.print(
             f"Your config file [purple]{config_filename}[/purple] appears to be already up-to-date for Nebari version [green]{__version__}[/green]"
         )
         return
     except (ValidationError, ValueError) as e:
-        if is_version_accepted(config.get("qhub_version", "")):
+        if is_version_accepted(config.get("nebari_version", "")):
             # There is an unrelated validation problem
             print(
                 f"Your config file {config_filename} appears to be already up-to-date for Nebari version {__version__} but there is another validation error.\n"
             )
             raise e
 
-    start_version = config.get("qhub_version", "")
+    start_version = config.get("nebari_version", "")
 
     UpgradeStep.upgrade(
         config, start_version, __version__, config_filename, attempt_fixes
     )
 
     # Backup old file
     backup_config_file(config_filename, f".{start_version or 'old'}")
@@ -141,15 +147,15 @@
 
         print(
             f"\n---> Starting upgrade from {start_version or 'old version'} to {finish_version}\n"
         )
 
         # Set the new version
         if start_version == "":
-            assert "qhub_version" not in config
+            assert "nebari_version" not in config
         assert self.version != start_version
 
         if self.requires_nebari_version_field():
             print(f"Setting nebari_version to {self.version}")
             config["nebari_version"] = self.version
 
         # Update images
@@ -376,14 +382,39 @@
 
             print(
                 f"Setting access type of JupyterLab profile {name} to {profile['access']}"
             )
         return config
 
 
+class Upgrade_2023_4_2(UpgradeStep):
+    version = "2023.4.2"
+
+    def _version_specific_upgrade(
+        self, config, start_version, config_filename: pathlib.Path, *args, **kwargs
+    ):
+        """
+        Prompt users to delete Argo CRDs
+        """
+
+        kubectl_delete_argo_crds_cmd = "kubectl delete crds clusterworkflowtemplates.argoproj.io cronworkflows.argoproj.io workfloweventbindings.argoproj.io workflows.argoproj.io workflowtasksets.argoproj.io workflowtemplates.argoproj.io"
+
+        rich.print(
+            f"\n\n[bold cyan]Note:[/] Upgrading requires a one-time manual deletion of the Argo Workflows Custom Resource Definitions (CRDs). \n\n[red bold]Warning:  [link=https://{config['domain']}/argo/workflows]Workflows[/link] and [link=https://{config['domain']}/argo/workflows]CronWorkflows[/link] created before deleting the CRDs will be erased when the CRDs are deleted and will not be restored.[/red bold] \n\nThe updated CRDs will be installed during the next [cyan bold]nebari deploy[/cyan bold] step. Argo Workflows will not function after deleting the CRDs until the updated CRDs are installed in the next nebari deploy. You must delete the Argo CRDs before upgrading to {self.version} or deploy step will fail.  Please delete them before proceeding by generating a kubeconfig (see [link=https://www.nebari.dev/docs/how-tos/debug-nebari/#generating-the-kubeconfig]docs[/link]), installing kubectl (see [link=https://www.nebari.dev/docs/how-tos/debug-nebari#installing-kubectl]docs[/link]), and running the following command:\n\n\t[cyan bold]{kubectl_delete_argo_crds_cmd} [/cyan bold]\n"
+            ""
+        )
+
+        continue_ = Prompt.ask("Have you deleted the Argo CRDs? [y/N]", default="N")
+        if not continue_ == "y":
+            print(f"You must delete the Argo CRDs before upgrading to {self.version}")
+            exit()
+
+        return config
+
+
 __rounded_version__ = ".".join([str(c) for c in rounded_ver_parse(__version__)])
 
 # Manually-added upgrade steps must go above this line
 if not UpgradeStep.has_step(__rounded_version__):
     # Always have a way to upgrade to the latest full version number, even if no customizations
     # Don't let dev/prerelease versions cloud things
     class UpgradeLatest(UpgradeStep):
```

### Comparing `nebari-2023.4.1a5/nebari/utils.py` & `nebari-2023.5.1rc1/nebari/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/version.py` & `nebari-2023.5.1rc1/nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/cli/dev.py` & `nebari-2023.5.1rc1/nebari/cli/dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/cli/init.py` & `nebari-2023.5.1rc1/nebari/cli/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,15 @@
             check_auth_provider_creds(ctx, auth_provider=inputs.auth_provider)
 
         if inputs.auth_provider.lower() == AuthenticationEnum.auth0.value.lower():
             inputs.auth_auto_provision = questionary.confirm(
                 "Would you like us to auto provision the Auth0 Machine-to-Machine app?",
                 default=False,
                 qmark=qmark,
+                auto_enter=False,
             ).unsafe_ask()
 
         elif inputs.auth_provider.lower() == AuthenticationEnum.github.value.lower():
             rich.print(
                 (
                     ":warning: If you haven't done so already, please ensure the following:\n"
                     f"The `Homepage URL` is set to: [green]https://{inputs.domain_name}[/green]\n"
@@ -420,14 +421,15 @@
                 "to automatically handle the future deployments of your infrastructure.\n\n"
             )
         )
         if questionary.confirm(
             "Would you like to adopt a GitOps approach to managing Nebari?",
             default=False,
             qmark=qmark,
+            auto_enter=False,
         ).unsafe_ask():
             repo_url = "http://{git_provider}/{org_name}/{repo_name}"
 
             git_provider = questionary.select(
                 "Which git provider would you like to use?",
                 choices=enum_to_list(GitRepoEnum),
                 qmark=qmark,
@@ -448,14 +450,15 @@
             )
 
             if git_provider == GitRepoEnum.github.value.lower():
                 inputs.repository_auto_provision = questionary.confirm(
                     f"Would you like nebari to create a remote repository on {git_provider}?",
                     default=False,
                     qmark=qmark,
+                    auto_enter=False,
                 ).unsafe_ask()
 
             if not disable_checks and inputs.repository_auto_provision:
                 check_repository_creds(ctx, git_provider)
 
             if git_provider == GitRepoEnum.github.value.lower():
                 inputs.ci_provider = CiEnum.github_actions.value.lower()
@@ -469,14 +472,15 @@
                 "all we need is an email address from you.\n\n"
             )
         )
         ssl_cert = questionary.confirm(
             "Would you like to add a Let's Encrypt SSL certificate to your domain?",
             default=False,
             qmark=qmark,
+            auto_enter=False,
         ).unsafe_ask()
 
         if ssl_cert:
             inputs.ssl_cert_email = questionary.text(
                 "Which email address should Let's Encrypt associate the certificate with?",
                 qmark=qmark,
             ).unsafe_ask()
@@ -493,14 +497,15 @@
                 "\n ⚠️  caution is advised!\n\n"
             )
         )
         if questionary.confirm(
             "Would you like to make advanced configuration changes?",
             default=False,
             qmark=qmark,
+            auto_enter=False,
         ).unsafe_ask():
             # TERRAFORM STATE
             inputs.terraform_state = questionary.select(
                 "Where should the Terraform State be provisioned?",
                 choices=enum_to_list(TerraformStateEnum),
                 qmark=qmark,
             ).unsafe_ask()
```

### Comparing `nebari-2023.4.1a5/nebari/cli/keycloak.py` & `nebari-2023.5.1rc1/nebari/cli/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/cli/main.py` & `nebari-2023.5.1rc1/nebari/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 )
 
 
 @app.callback(invoke_without_command=True)
 def version(
     version: Optional[bool] = typer.Option(
         None,
-        "-v",
+        "-V",
         "--version",
         help="Nebari version number",
         is_eager=True,
     ),
 ):
     if version:
         print(__version__)
```

### Comparing `nebari-2023.4.1a5/nebari/provider/git.py` & `nebari-2023.5.1rc1/nebari/provider/git.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/terraform.py` & `nebari-2023.5.1rc1/nebari/provider/terraform.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/cicd/github.py` & `nebari-2023.5.1rc1/nebari/provider/cicd/github.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/cicd/gitlab.py` & `nebari-2023.5.1rc1/nebari/provider/cicd/gitlab.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/cicd/linter.py` & `nebari-2023.5.1rc1/nebari/provider/cicd/linter.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/cloud/amazon_web_services.py` & `nebari-2023.5.1rc1/nebari/provider/cloud/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/cloud/azure_cloud.py` & `nebari-2023.5.1rc1/nebari/provider/cloud/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/cloud/digital_ocean.py` & `nebari-2023.5.1rc1/nebari/provider/cloud/digital_ocean.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/cloud/google_cloud.py` & `nebari-2023.5.1rc1/nebari/provider/cloud/google_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/dns/cloudflare.py` & `nebari-2023.5.1rc1/nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/provider/oauth/auth0.py` & `nebari-2023.5.1rc1/nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/stages/checks.py` & `nebari-2023.5.1rc1/nebari/stages/checks.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/stages/input_vars.py` & `nebari-2023.5.1rc1/nebari/stages/input_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import json
 import os
 import tempfile
 from urllib.parse import urlencode
 
-from nebari.constants import DEFAULT_CONDA_STORE_IMAGE_TAG, DEFAULT_TRAEFIK_IMAGE_TAG
+from nebari.constants import (
+    DEFAULT_CONDA_STORE_IMAGE_TAG,
+    DEFAULT_GKE_RELEASE_CHANNEL,
+    DEFAULT_TRAEFIK_IMAGE_TAG,
+)
 
 
 def stage_01_terraform_state(stage_outputs, config):
     if config["provider"] == "do":
         return {
             "name": config["project_name"],
             "namespace": config["namespace"],
@@ -61,14 +65,17 @@
     elif config["provider"] == "gcp":
         return {
             "name": config["project_name"],
             "environment": config["namespace"],
             "region": config["google_cloud_platform"]["region"],
             "project_id": config["google_cloud_platform"]["project"],
             "kubernetes_version": config["google_cloud_platform"]["kubernetes_version"],
+            "release_channel": config.get("google_cloud_platform", {}).get(
+                "release_channel", DEFAULT_GKE_RELEASE_CHANNEL
+            ),
             "node_groups": [
                 {
                     "name": key,
                     "instance_type": value["instance"],
                     "min_size": value["min_nodes"],
                     "max_size": value["max_nodes"],
                     "guest_accelerators": value["guest_accelerators"]
@@ -281,26 +288,32 @@
         "conda-store-filesystem-storage": config["storage"]["conda_store"],
         "conda-store-service-token-scopes": {
             "cdsdashboards": {
                 "primary_namespace": "cdsdashboards",
                 "role_bindings": {
                     "*/*": ["viewer"],
                 },
-            }
+            },
+            "dask-gateway": {
+                "primary_namespace": "",
+                "role_bindings": {
+                    "*/*": ["viewer"],
+                },
+            },
         },
         "conda-store-default-namespace": config.get("conda_store", {}).get(
             "default_namespace", "nebari-git"
         ),
         "conda-store-extra-settings": config.get("conda_store", {}).get(
             "extra_settings", {}
         ),
         "conda-store-extra-config": config.get("conda_store", {}).get(
             "extra_config", ""
         ),
-        "conda-store-image-tag": config.get("conda-store", {}).get(
+        "conda-store-image-tag": config.get("conda_store", {}).get(
             "image_tag", DEFAULT_CONDA_STORE_IMAGE_TAG
         ),
         # jupyterhub
         "cdsdashboards": config["cdsdashboards"],
         "jupyterhub-theme": jupyterhub_theme,
         "jupyterhub-image": _split_docker_image_name(
             config["default_images"]["jupyterhub"]
```

### Comparing `nebari-2023.4.1a5/nebari/stages/state_imports.py` & `nebari-2023.5.1rc1/nebari/stages/state_imports.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/stages/tf_objects.py` & `nebari-2023.5.1rc1/nebari/stages/tf_objects.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/main.tf`

 * *Files 16% similar despite different names*

```diff
@@ -29,8 +29,9 @@
   node_groups                       = var.node_groups
   network                           = var.network
   subnetwork                        = var.subnetwork
   ip_allocation_policy              = var.ip_allocation_policy
   master_authorized_networks_config = var.master_authorized_networks_config
   private_cluster_config            = var.private_cluster_config
   kubernetes_version                = var.kubernetes_version
+  release_channel                   = var.release_channel
 }
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/variables.tf`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 }
 
 variable "kubernetes_version" {
   description = "Kubernetes version for GKE cluster"
   type        = string
 }
 
+variable "release_channel" {
+  description = "The cadence of GKE version upgrades"
+  type        = string
+}
+
 variable "networking_mode" {
   description = "Determines whether alias IPs or routes will be used for pod IPs in the cluster. Options are VPC_NATIVE or ROUTES."
   type        = string
   default     = "ROUTES"
 }
 
 variable "network" {
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   master_auth {
     client_certificate_config {
       issue_client_certificate = true
     }
   }
 
   release_channel {
-    channel = "UNSPECIFIED"
+    channel = var.release_channel
   }
 
   networking_mode = var.networking_mode
   network         = var.network
   subnetwork      = var.subnetwork
 
   dynamic "ip_allocation_policy" {
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 }
 
 variable "kubernetes_version" {
   description = "Kubernetes version for GKE cluster"
   type        = string
 }
 
+variable "release_channel" {
+  description = "The cadence of GKE version upgrades"
+  type        = string
+}
+
 variable "node_groups" {
   description = "Node groups to add to GCP Kubernetes Cluster"
   type        = any
   default = [
     {
       name          = "general"
       instance_type = "n1-standard-2"
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/metallb.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/02-infrastructure/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
   namespace = var.namespace
 
   repository = "https://codecentric.github.io/helm-charts"
   chart      = "keycloak"
   version    = "15.0.2"
 
   values = concat([
+    # https://github.com/codecentric/helm-charts/blob/keycloak-15.0.2/charts/keycloak/values.yaml
     file("${path.module}/values.yaml"),
     jsonencode({
       nodeSelector = {
         "${var.node-group.key}" = var.node-group.value
       }
       postgresql = {
         primary = {
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf`

 * *Files 17% similar despite different names*

```diff
@@ -42,7 +42,24 @@
 resource "keycloak_default_groups" "default" {
   realm_id = keycloak_realm.main.id
   group_ids = [
     for g in var.default_groups :
     keycloak_group.groups[g].id
   ]
 }
+
+# needed for keycloak monitoring to function
+resource "keycloak_realm_events" "realm_events" {
+  realm_id = keycloak_realm.main.id
+
+  events_enabled = true
+
+  admin_events_enabled         = true
+  admin_events_details_enabled = true
+
+  # When omitted or left empty, keycloak will enable all event types
+  enabled_event_types = []
+
+  events_listeners = [
+    "jboss-logging", "metrics-listener",
+  ]
+}
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf` & `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf` & `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/argo-workflows.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/argo-workflows.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/clearml.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/clearml.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/conda-store.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/conda-store.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/dask_gateway.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/dask_gateway.tf`

 * *Files 20% similar despite different names*

```diff
@@ -31,11 +31,13 @@
   # needs to match name in module.jupyterhub.extra-mounts
   dask-etc-configmap-name = "dask-etc"
 
   # environments
   conda-store-pvc               = module.conda-store-nfs-mount.persistent_volume_claim.name
   conda-store-mount             = "/home/conda"
   default-conda-store-namespace = var.conda-store-default-namespace
+  conda-store-api-token         = module.kubernetes-conda-store-server.service-tokens.dask-gateway
+  conda-store-service-name      = module.kubernetes-conda-store-server.service_name
 
   # profiles
   profiles = var.dask-gateway-profiles
 }
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/jupyterhub.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/jupyterhub.tf`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
       kind      = "configmap"
     },
   }
 
   services = concat([
     "dask-gateway"
     ],
+    (var.monitoring-enabled ? ["monitoring"] : []),
     (var.prefect-enabled ? ["prefect"] : []),
     (var.kbatch-enabled ? ["kbatch"] : [])
   )
 
   general-node-group = var.node_groups.general
   user-node-group    = var.node_groups.user
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/kbatch.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/kbatch.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/prefect.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/prefect.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 }
 
 resource "helm_release" "argo-workflows" {
   name       = local.name
   namespace  = var.namespace
   repository = "https://argoproj.github.io/argo-helm"
   chart      = "argo-workflows"
-  version    = "0.13.1"
+  version    = "0.22.9"
 
   values = concat([
     file("${path.module}/values.yaml"),
-    # https://github.com/argoproj/argo-helm/blob/argo-workflows-0.13.1/charts/argo-workflows/values.yaml
-
 
     jsonencode({
       singleNamespace = true # Restrict Argo to operate only in a single namespace (the namespace of the Helm release)
 
       controller = {
         metricsConfig = {
           enabled = true # enable prometheus
@@ -58,17 +56,14 @@
           customGroupClaimName = "roles"
           scopes               = ["roles"]
         }
         nodeSelector = {
           "${var.node-group.key}" = var.node-group.value
         }
       }
-      controller = {
-        containerRuntimeExecutor = "emissary"
-      }
 
     })
   ], var.overrides)
 }
 
 resource "kubernetes_secret" "argo-oidc-secret" {
   metadata {
@@ -148,90 +143,125 @@
           ]
         }
       ]
     }
   }
 }
 
-resource "kubernetes_service_account" "argo-admin-sa" {
+resource "kubernetes_service_account_v1" "argo-admin-sa" {
   metadata {
     name      = "argo-admin"
     namespace = var.namespace
     annotations = {
       "workflows.argoproj.io/rbac-rule" : "'argo_admin' in groups"
       "workflows.argoproj.io/rbac-rule-precedence" : "11"
     }
   }
 }
 
+resource "kubernetes_secret_v1" "argo_admin_sa_token" {
+  metadata {
+    name      = "argo-admin.service-account-token"
+    namespace = var.namespace
+    annotations = {
+      "kubernetes.io/service-account.name" = kubernetes_service_account_v1.argo-admin-sa.metadata[0].name
+
+    }
+  }
+  type = "kubernetes.io/service-account-token"
+}
+
 resource "kubernetes_cluster_role_binding" "argo-admin-rb" {
   metadata {
     name = "argo-admin"
   }
 
   role_ref {
     api_group = "rbac.authorization.k8s.io"
     kind      = "ClusterRole"
     name      = "argo-workflows-admin" # role deployed as part of helm chart
   }
   subject {
     kind      = "ServiceAccount"
-    name      = kubernetes_service_account.argo-admin-sa.metadata.0.name
+    name      = kubernetes_service_account_v1.argo-admin-sa.metadata.0.name
     namespace = var.namespace
   }
 }
 
-resource "kubernetes_service_account" "argo-edit-sa" {
+resource "kubernetes_service_account_v1" "argo-dev-sa" {
   metadata {
-    name      = "argo-edit"
+    name      = "argo-dev"
     namespace = var.namespace
     annotations = {
       "workflows.argoproj.io/rbac-rule" : "'argo_developer' in groups"
       "workflows.argoproj.io/rbac-rule-precedence" : "10"
     }
+  }
+}
 
+resource "kubernetes_secret_v1" "argo_dev_sa_token" {
+  metadata {
+    name      = "argo-dev.service-account-token"
+    namespace = var.namespace
+    annotations = {
+      "kubernetes.io/service-account.name" = kubernetes_service_account_v1.argo-dev-sa.metadata[0].name
+    }
   }
+  type = "kubernetes.io/service-account-token"
 }
 
-resource "kubernetes_cluster_role_binding" "argo-edit-rb" {
+resource "kubernetes_cluster_role_binding" "argo-dev-rb" {
   metadata {
-    name = "argo-edit"
+    name = "argo-dev"
   }
 
   role_ref {
     api_group = "rbac.authorization.k8s.io"
     kind      = "ClusterRole"
     name      = "argo-workflows-edit" # role deployed as part of helm chart
   }
   subject {
     kind      = "ServiceAccount"
-    name      = kubernetes_service_account.argo-edit-sa.metadata.0.name
+    name      = kubernetes_service_account_v1.argo-dev-sa.metadata.0.name
     namespace = var.namespace
   }
 }
-resource "kubernetes_service_account" "argo-view-sa" {
+
+
+resource "kubernetes_service_account_v1" "argo-view-sa" {
   metadata {
-    name      = "argo-view"
+    name      = "argo-viewer"
     namespace = var.namespace
     annotations = {
       "workflows.argoproj.io/rbac-rule" : "'argo_viewer' in groups"
       "workflows.argoproj.io/rbac-rule-precedence" : "9"
     }
   }
 }
 
+resource "kubernetes_secret_v1" "argo_viewer_sa_token" {
+  metadata {
+    name      = "argo-viewer.service-account-token"
+    namespace = var.namespace
+    annotations = {
+      "kubernetes.io/service-account.name" = kubernetes_service_account_v1.argo-view-sa.metadata[0].name
+    }
+  }
+  type = "kubernetes.io/service-account-token"
+}
+
 resource "kubernetes_cluster_role_binding" "argo-view-rb" {
   metadata {
     name = "argo-view"
   }
 
   role_ref {
     api_group = "rbac.authorization.k8s.io"
     kind      = "ClusterRole"
     name      = "argo-workflows-view" # role deployed as part of helm chart
   }
   subject {
     kind      = "ServiceAccount"
-    name      = kubernetes_service_account.argo-view-sa.metadata.0.name
+    name      = kubernetes_service_account_v1.argo-view-sa.metadata.0.name
     namespace = var.namespace
   }
 }
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,18 @@
 }
 
 
 resource "kubernetes_service" "server" {
   metadata {
     name      = "${var.name}-conda-store-server"
     namespace = var.namespace
+    labels = {
+      app       = "conda-store"
+      component = "conda-store-server"
+    }
   }
 
   spec {
     selector = {
       role = "${var.name}-conda-store-server"
     }
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
       cluster                              = var.cluster
       cluster-image                        = var.cluster-image
       profiles                             = var.profiles
       default-conda-store-namespace        = var.default-conda-store-namespace
       conda-store-pvc                      = var.conda-store-pvc
       conda-store-mount                    = var.conda-store-mount
       worker-node-group                    = var.worker-node-group
+      conda-store-api-token                = var.conda-store-api-token
+      conda-store-service-name             = var.conda-store-service-name
+      conda-store-namespace                = var.namespace
     })
   }
 }
 
 
 resource "kubernetes_config_map" "gateway" {
   metadata {
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files 3% similar despite different names*

```diff
@@ -185,7 +185,17 @@
   type        = string
 }
 
 variable "default-conda-store-namespace" {
   description = "Default conda-store namespace"
   type        = string
 }
+
+variable "conda-store-api-token" {
+  description = "Service token for conda-store api"
+  type        = string
+}
+
+variable "conda-store-service-name" {
+  description = "internal service-name:port where conda-store can be reached"
+  type        = string
+}
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import json
 import os
 
+import urllib3
 from aiohttp import web
 from dask_gateway_server.auth import JupyterHubAuthenticator
 from dask_gateway_server.options import Mapping, Options, Select
 
 
 def dask_gateway_config(path="/var/lib/dask-gateway/config.json"):
     with open(path) as f:
@@ -82,43 +83,35 @@
 
 c.DaskGateway.authenticator_class = NebariAuthentication
 c.JupyterHubAuthenticator.jupyterhub_api_url = config["jupyterhub_api_url"]
 c.JupyterHubAuthenticator.jupyterhub_api_token = config["jupyterhub_api_token"]
 
 
 # ==================== Profiles =======================
-def get_packages(conda_prefix):
-    try:
-        packages = set()
-        for filename in os.listdir(os.path.join(conda_prefix, "conda-meta")):
-            if filename.endswith(".json"):
-                with open(os.path.join(conda_prefix, "conda-meta", filename)) as f:
-                    packages.add(json.load(f).get("name"))
-        return packages
-    except OSError as e:
-        import logging
-
-        logger = logging.getLogger()
-        logger.error(f"An issue with a conda environment was encountered.\n{e}")
-
-
-def get_conda_prefixes(conda_store_mount):
-    for namespace in os.listdir(conda_store_mount):
-        if os.path.isdir(os.path.join(conda_store_mount, namespace, "envs")):
-            for name in os.listdir(os.path.join(conda_store_mount, namespace, "envs")):
-                yield namespace, name, os.path.join(
-                    conda_store_mount, namespace, "envs", name
-                )
-
-
-def list_dask_environments(conda_store_mount):
-    for namespace, name, conda_prefix in get_conda_prefixes(conda_store_mount):
-        packages = get_packages(conda_prefix)
-        if packages and {"dask", "distributed"} <= packages:
-            yield namespace, name, conda_prefix
+def list_dask_environments():
+    necessary_dask_packages = {"dask", "distributed", "dask-gateway"}
+    token = config["conda-store-api-token"]
+    conda_store_service_name, conda_store_service_port = config[
+        "conda-store-service-name"
+    ].split(":")
+    conda_store_endpoint = f"{conda_store_service_name}.{config['conda-store-namespace']}.svc:{conda_store_service_port}"
+    environment_endpoint = "/conda-store/api/v1/environment/"
+    query_params = f"?packages={'&packages='.join(necessary_dask_packages)}"
+
+    url = "http://" + conda_store_endpoint + environment_endpoint + query_params
+
+    http = urllib3.PoolManager()
+    response = http.request("GET", url, headers={"Authorization": f"Bearer {token}"})
+
+    # parse response
+    j = json.loads(response.data.decode("UTF-8"))
+    return [
+        (conda_env["namespace"]["name"], conda_env["name"])
+        for conda_env in j.get("data", [])
+    ]
 
 
 def base_node_group(options):
     default_node_group = {
         config["worker-node-group"]["key"]: config["worker-node-group"]["value"]
     }
 
@@ -247,29 +240,27 @@
 
 
 def user_options(user):
     default_namespace = config["default-conda-store-namespace"]
     allowed_namespaces = set(
         [default_namespace, "global", user.name] + list(user.groups)
     )
-    environments = {
-        f"{namespace}/{name}": conda_prefix
-        for namespace, name, conda_prefix in list_dask_environments(
-            config["conda-store-mount"]
-        )
-        if namespace in allowed_namespaces
-    }
+    conda_environments = []
+    for namespace, name in list_dask_environments():
+        if namespace not in allowed_namespaces:
+            continue
+        conda_environments.append(f"{namespace}/{namespace}-{name}")
 
     args = []
-    if environments:
+    if conda_environments:
         args += [
             Select(
                 "conda_environment",
-                list(environments.keys()),
-                default=list(environments.keys())[0],
+                conda_environments,
+                default=conda_environments[0],
                 label="Environment",
             )
         ]
     if config["profiles"]:
         args += [
             Select(
                 "profile",
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# https://github.com/jupyterhub/zero-to-jupyterhub-k8s/blob/main/jupyterhub/values.yaml
+# https://github.com/jupyterhub/zero-to-jupyterhub-k8s/blob/1.2.0/jupyterhub/values.yaml
 hub:
   db:
     type: sqlite-pvc
     pvc:
       storage: 1Gi
   baseUrl: "/"
   networkPolicy:
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/conda_store.json` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9282857674319729%*

 * *Differences: {"'panels'": "{1: {'fieldConfig': {'defaults': {'min': 0}}, 'targets': {0: {'legendFormat': "*

 * *             "'conda_store_build_queued'}, 1: {'legendFormat': 'conda_store_build_building'}, 2: "*

 * *             "{'legendFormat': 'conda_store_build_completed'}, 3: {'legendFormat': "*

 * *             "'conda_store_build_failed'}}, delete: ['datasource']}}",*

 * * "'version'": '1',*

 * * 'delete': "['id']"}*

```diff
@@ -18,15 +18,14 @@
             }
         ]
     },
     "description": "",
     "editable": true,
     "fiscalYearStartMonth": 0,
     "graphTooltip": 0,
-    "id": 5,
     "links": [],
     "liveNow": false,
     "panels": [
         {
             "collapsed": false,
             "gridPos": {
                 "h": 1,
@@ -36,18 +35,14 @@
             },
             "id": 6,
             "panels": [],
             "title": "Environments",
             "type": "row"
         },
         {
-            "datasource": {
-                "type": "prometheus",
-                "uid": "PBFA97CFB590B2093"
-            },
             "fieldConfig": {
                 "defaults": {
                     "color": {
                         "mode": "palette-classic"
                     },
                     "custom": {
                         "axisLabel": "",
@@ -74,14 +69,15 @@
                             "mode": "none"
                         },
                         "thresholdsStyle": {
                             "mode": "off"
                         }
                     },
                     "mappings": [],
+                    "min": 0,
                     "noValue": "0",
                     "thresholds": {
                         "mode": "absolute",
                         "steps": [
                             {
                                 "color": "green",
                                 "value": null
@@ -117,53 +113,53 @@
                     "datasource": {
                         "type": "prometheus",
                         "uid": "PBFA97CFB590B2093"
                     },
                     "exemplar": true,
                     "expr": "conda_store_build_queued",
                     "interval": "",
-                    "legendFormat": "",
+                    "legendFormat": "conda_store_build_queued",
                     "refId": "Queued"
                 },
                 {
                     "datasource": {
                         "type": "prometheus",
                         "uid": "PBFA97CFB590B2093"
                     },
                     "exemplar": true,
                     "expr": "conda_store_build_building",
                     "hide": false,
                     "instant": false,
                     "interval": "",
-                    "legendFormat": "",
+                    "legendFormat": "conda_store_build_building",
                     "refId": "Building"
                 },
                 {
                     "datasource": {
                         "type": "prometheus",
                         "uid": "PBFA97CFB590B2093"
                     },
                     "exemplar": true,
                     "expr": "conda_store_build_completed",
                     "hide": false,
                     "instant": false,
                     "interval": "",
-                    "legendFormat": "",
+                    "legendFormat": "conda_store_build_completed",
                     "refId": "Completed"
                 },
                 {
                     "datasource": {
                         "type": "prometheus",
                         "uid": "PBFA97CFB590B2093"
                     },
                     "exemplar": true,
                     "expr": "conda_store_build_failed",
                     "hide": false,
                     "interval": "",
-                    "legendFormat": "",
+                    "legendFormat": "conda_store_build_failed",
                     "refId": "Failed"
                 }
             ],
             "title": "Builds",
             "type": "timeseries"
         },
         {
@@ -716,10 +712,10 @@
         "from": "now-6h",
         "to": "now"
     },
     "timepicker": {},
     "timezone": "",
     "title": "Conda-Store",
     "uid": "7lHPaT1nz",
-    "version": 5,
+    "version": 1,
     "weekStart": ""
 }
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/keycloak.json` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998562635281385%*

 * *Differences: {"'panels'": '{0: {\'targets\': {0: {\'expr\': \'sum(jvm_memory_bytes_used{pod="$instance", '*

 * *             'area="heap"})*100/sum(jvm_memory_bytes_max{pod="$instance", area="heap"})\'}}}, 1: '*

 * *             '{\'targets\': {0: {\'expr\': \'sum(jvm_memory_bytes_used{pod="$instance", '*

 * *             'area="nonheap"})*100/sum(jvm_memory_bytes_max{pod="$instance", '*

 * *             'area="nonheap"})\'}}}, 2: {\'targets\': {0: {\'expr\': '*

 * *             '\'sum(jvm_memory_bytes_max{pod="$instance"})\'}, 1: {\'expr\': '*

 * * […]*

```diff
@@ -167,15 +167,15 @@
                 "showThresholdLabels": false,
                 "showThresholdMarkers": true
             },
             "pluginVersion": "8.3.3",
             "span": 0,
             "targets": [
                 {
-                    "expr": "sum(jvm_memory_bytes_used{kubernetes_pod_name=\"$instance\", area=\"heap\"})*100/sum(jvm_memory_bytes_max{kubernetes_pod_name=\"$instance\", area=\"heap\"})",
+                    "expr": "sum(jvm_memory_bytes_used{pod=\"$instance\", area=\"heap\"})*100/sum(jvm_memory_bytes_max{pod=\"$instance\", area=\"heap\"})",
                     "interval": "",
                     "legendFormat": "",
                     "refId": "A"
                 }
             ],
             "title": "Current Memory HEAP",
             "type": "gauge"
@@ -301,15 +301,15 @@
                 "showThresholdLabels": false,
                 "showThresholdMarkers": true
             },
             "pluginVersion": "8.3.3",
             "span": 0,
             "targets": [
                 {
-                    "expr": "sum(jvm_memory_bytes_used{kubernetes_pod_name=\"$instance\", area=\"nonheap\"})*100/sum(jvm_memory_bytes_max{kubernetes_pod_name=\"$instance\", area=\"nonheap\"})",
+                    "expr": "sum(jvm_memory_bytes_used{pod=\"$instance\", area=\"nonheap\"})*100/sum(jvm_memory_bytes_max{pod=\"$instance\", area=\"nonheap\"})",
                     "interval": "",
                     "legendFormat": "",
                     "refId": "A"
                 }
             ],
             "title": "Current Memory nonHEAP",
             "type": "gauge"
@@ -387,31 +387,31 @@
                 "tooltip": {
                     "mode": "single"
                 }
             },
             "pluginVersion": "8.3.3",
             "targets": [
                 {
-                    "expr": "sum(jvm_memory_bytes_max{kubernetes_pod_name=\"$instance\"})",
+                    "expr": "sum(jvm_memory_bytes_max{pod=\"$instance\"})",
                     "format": "time_series",
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "Max",
                     "refId": "A"
                 },
                 {
-                    "expr": "sum(jvm_memory_bytes_committed{kubernetes_pod_name=\"$instance\"})",
+                    "expr": "sum(jvm_memory_bytes_committed{pod=\"$instance\"})",
                     "format": "time_series",
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "Comitted",
                     "refId": "C"
                 },
                 {
-                    "expr": "sum(jvm_memory_bytes_used{kubernetes_pod_name=\"$instance\"})",
+                    "expr": "sum(jvm_memory_bytes_used{pod=\"$instance\"})",
                     "format": "time_series",
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "Used",
                     "refId": "B"
                 }
             ],
@@ -1408,15 +1408,15 @@
                 {
                     "expr": "sum by (realm)(increase(keycloak_registrations{provider=\"keycloak\",realm=\"$realm\"} [30m]))",
                     "interval": "",
                     "legendFormat": "Sum by {{realm}}",
                     "refId": "B"
                 }
             ],
-            "title": "Registrations per CLIENT on relm $realm",
+            "title": "Registrations per CLIENT on Realm $realm",
             "type": "timeseries"
         },
         {
             "datasource": {
                 "uid": "$Datasource"
             },
             "fieldConfig": {
@@ -2037,24 +2037,24 @@
                     "selected": false,
                     "text": "None",
                     "value": ""
                 },
                 "datasource": {
                     "uid": "$Datasource"
                 },
-                "definition": "label_values(keycloak_logins,kubernetes_pod_name)",
+                "definition": "label_values(keycloak_logins,pod)",
                 "hide": 0,
                 "includeAll": false,
                 "label": "Instance",
                 "multi": false,
                 "multiFormat": "",
                 "name": "instance",
                 "options": [],
                 "query": {
-                    "query": "label_values(keycloak_logins,kubernetes_pod_name)",
+                    "query": "label_values(keycloak_logins,pod)",
                     "refId": "Prometheus-instance-Variable-Query"
                 },
                 "refresh": 1,
                 "regex": "",
                 "skipUrlSync": false,
                 "sort": 0,
                 "tagValuesQuery": "",
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/traefik.json` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7279824111788321%*

 * *Differences: {"'annotations'": "{'list': {0: {'target': OrderedDict([('limit', 100), ('matchAny', False), "*

 * *                  "('tags', []), ('type', 'dashboard')])}}}",*

 * * "'fiscalYearStartMonth'": '0',*

 * * "'iteration'": '1681240333933',*

 * * "'liveNow'": 'False',*

 * * "'panels'": "{0: {'datasource': {replace: OrderedDict([('type', 'prometheus'), ('uid', "*

 * *             "'PBFA97CFB590B2093')])}}, 1: {'pluginVersion': '8.3.3', 'targets': {0: {'expr': "*

 * *             '\'count(kube_pod_status_ready{namespace="$namespace",condition="tru […]*

```diff
@@ -4,43 +4,51 @@
             {
                 "builtIn": 1,
                 "datasource": "-- Grafana --",
                 "enable": true,
                 "hide": true,
                 "iconColor": "rgba(0, 211, 255, 1)",
                 "name": "Annotations & Alerts",
+                "target": {
+                    "limit": 100,
+                    "matchAny": false,
+                    "tags": [],
+                    "type": "dashboard"
+                },
                 "type": "dashboard"
             }
         ]
     },
     "description": "Traefik Metrics Overview",
     "editable": true,
+    "fiscalYearStartMonth": 0,
     "gnetId": 13165,
     "graphTooltip": 1,
-    "id": 27,
-    "iteration": 1630948875428,
+    "iteration": 1681240333933,
     "links": [],
+    "liveNow": false,
     "panels": [
         {
             "collapsed": false,
-            "datasource": "Prometheus",
+            "datasource": {
+                "type": "prometheus",
+                "uid": "PBFA97CFB590B2093"
+            },
             "gridPos": {
                 "h": 1,
                 "w": 24,
                 "x": 0,
                 "y": 0
             },
             "id": 21,
             "panels": [],
             "title": "General",
             "type": "row"
         },
         {
-            "cacheTimeout": null,
-            "datasource": null,
             "fieldConfig": {
                 "defaults": {
                     "color": {
                         "fixedColor": "rgb(31, 120, 193)",
                         "mode": "fixed"
                     },
                     "mappings": [
@@ -74,15 +82,14 @@
             "gridPos": {
                 "h": 7,
                 "w": 3,
                 "x": 0,
                 "y": 1
             },
             "id": 13,
-            "interval": null,
             "links": [],
             "maxDataPoints": 100,
             "options": {
                 "colorMode": "none",
                 "graphMode": "area",
                 "justifyMode": "auto",
                 "orientation": "horizontal",
@@ -92,19 +99,23 @@
                     ],
                     "fields": "",
                     "values": false
                 },
                 "text": {},
                 "textMode": "auto"
             },
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "targets": [
                 {
+                    "datasource": {
+                        "type": "prometheus",
+                        "uid": "PBFA97CFB590B2093"
+                    },
                     "exemplar": true,
-                    "expr": "count(kube_pod_status_ready{namespace=\"$namespace\",condition=\"true\",pod=~\".*traefik.*\", job=\"traefik\"})",
+                    "expr": "count(kube_pod_status_ready{namespace=\"$namespace\",condition=\"true\",pod=~\"nebari-traefik-ingress-.*\", job=\"kube-state-metrics\"})",
                     "format": "time_series",
                     "hide": false,
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "",
                     "refId": "A"
                 }
@@ -113,15 +124,14 @@
             "type": "stat"
         },
         {
             "aliasColors": {},
             "bars": false,
             "dashLength": 10,
             "dashes": false,
-            "datasource": null,
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 7,
                 "w": 21,
                 "x": 3,
                 "y": 1
@@ -143,15 +153,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": false,
             "steppedLine": false,
@@ -163,57 +173,50 @@
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "{{ instance }}",
                     "refId": "A"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Per instance latency $percentiles th perc over 5 min",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "format": "s",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
-                    "min": null,
                     "show": false
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "collapsed": false,
-            "datasource": "Prometheus",
+            "datasource": {
+                "type": "prometheus",
+                "uid": "PBFA97CFB590B2093"
+            },
             "gridPos": {
                 "h": 1,
                 "w": 24,
                 "x": 0,
                 "y": 8
             },
             "id": 17,
@@ -222,15 +225,17 @@
             "type": "row"
         },
         {
             "aliasColors": {},
             "bars": false,
             "dashLength": 10,
             "dashes": false,
-            "datasource": "$Prometheus",
+            "datasource": {
+                "uid": "$Prometheus"
+            },
             "fill": 7,
             "fillGradient": 0,
             "gridPos": {
                 "h": 7,
                 "w": 12,
                 "x": 0,
                 "y": 9
@@ -255,15 +260,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": true,
             "steppedLine": false,
@@ -275,61 +280,54 @@
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "{{ method }}",
                     "refId": "A"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Open Connections",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "decimals": 0,
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": false
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "aliasColors": {},
             "bars": false,
             "dashLength": 10,
             "dashes": false,
-            "datasource": "$Prometheus",
+            "datasource": {
+                "uid": "$Prometheus"
+            },
             "decimals": 2,
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 7,
                 "w": 12,
                 "x": 12,
@@ -342,27 +340,26 @@
                 "avg": true,
                 "current": true,
                 "hideZero": true,
                 "max": false,
                 "min": false,
                 "rightSide": true,
                 "show": true,
-                "sideWidth": null,
                 "total": false,
                 "values": true
             },
             "lines": true,
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": false,
             "steppedLine": false,
@@ -374,61 +371,52 @@
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "Code 200",
                     "refId": "A"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Apdex score (over 5 min)",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "decimals": 2,
                     "format": "short",
                     "label": "",
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": false
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "aliasColors": {},
             "bars": true,
             "dashLength": 10,
             "dashes": false,
-            "datasource": null,
             "decimals": 2,
             "description": "",
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 10,
                 "w": 24,
@@ -455,15 +443,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": false,
             "steppedLine": false,
@@ -475,59 +463,55 @@
                     "interval": "",
                     "intervalFactor": 2,
                     "legendFormat": "{{ entrypoint }}",
                     "refId": "A"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Requests/min per entrypoint",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "decimals": 2,
                     "format": "short",
                     "label": "",
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "decimals": 2,
                     "format": "short",
                     "label": "",
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "collapsed": false,
-            "datasource": "Prometheus",
+            "datasource": {
+                "type": "prometheus",
+                "uid": "PBFA97CFB590B2093"
+            },
             "gridPos": {
                 "h": 1,
                 "w": 24,
                 "x": 0,
                 "y": 26
             },
             "id": 24,
@@ -536,15 +520,17 @@
             "type": "row"
         },
         {
             "aliasColors": {},
             "bars": false,
             "dashLength": 10,
             "dashes": false,
-            "datasource": "$Prometheus",
+            "datasource": {
+                "uid": "$Prometheus"
+            },
             "decimals": 0,
             "fill": 7,
             "fillGradient": 0,
             "gridPos": {
                 "h": 7,
                 "w": 12,
                 "x": 0,
@@ -570,15 +556,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": true,
             "steppedLine": false,
@@ -590,61 +576,52 @@
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "{{ method }}",
                     "refId": "A"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Open Connections",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "decimals": 0,
                     "format": "short",
                     "label": "",
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": false
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "aliasColors": {},
             "bars": false,
             "dashLength": 10,
             "dashes": false,
-            "datasource": null,
             "decimals": 2,
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 7,
                 "w": 12,
                 "x": 12,
@@ -667,15 +644,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": false,
             "steppedLine": false,
@@ -695,61 +672,51 @@
                     "hide": false,
                     "interval": "",
                     "legendFormat": "",
                     "refId": "B"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Apdex score (over 5 min)",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "decimals": 2,
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": false
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "aliasColors": {},
             "bars": true,
             "dashLength": 10,
             "dashes": false,
-            "datasource": null,
             "decimals": 2,
             "description": "",
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 10,
                 "w": 24,
@@ -776,15 +743,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": false,
             "steppedLine": false,
@@ -796,59 +763,55 @@
                     "interval": "",
                     "intervalFactor": 2,
                     "legendFormat": "{{ service }}",
                     "refId": "A"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Requests/min per service",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "decimals": 2,
                     "format": "short",
                     "label": "",
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "decimals": 2,
                     "format": "short",
                     "label": "",
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "collapsed": false,
-            "datasource": "Prometheus",
+            "datasource": {
+                "type": "prometheus",
+                "uid": "PBFA97CFB590B2093"
+            },
             "gridPos": {
                 "h": 1,
                 "w": 24,
                 "x": 0,
                 "y": 44
             },
             "id": 15,
@@ -857,51 +820,51 @@
             "type": "row"
         },
         {
             "aliasColors": {},
             "bars": true,
             "dashLength": 10,
             "dashes": false,
-            "datasource": "$Prometheus",
+            "datasource": {
+                "uid": "$Prometheus"
+            },
             "decimals": 0,
             "description": "",
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 9,
                 "w": 12,
                 "x": 0,
                 "y": 45
             },
             "hiddenSeries": false,
             "id": 5,
-            "interval": null,
             "legend": {
                 "alignAsTable": true,
                 "avg": false,
                 "current": false,
                 "hideEmpty": false,
                 "hideZero": true,
                 "max": false,
                 "min": false,
                 "rightSide": true,
                 "show": true,
-                "sideWidth": null,
                 "total": true,
                 "values": true
             },
             "lines": false,
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": true,
             "steppedLine": false,
@@ -913,59 +876,53 @@
                     "interval": "1",
                     "intervalFactor": 2,
                     "legendFormat": "{{method}} : {{code}}",
                     "refId": "A"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Status method/codes over 5min",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "decimals": 2,
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 },
                 {
                     "decimals": 2,
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
                     "min": "0",
                     "show": true
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "collapsed": false,
-            "datasource": "Prometheus",
+            "datasource": {
+                "type": "prometheus",
+                "uid": "PBFA97CFB590B2093"
+            },
             "gridPos": {
                 "h": 1,
                 "w": 24,
                 "x": 0,
                 "y": 54
             },
             "id": 35,
@@ -974,15 +931,14 @@
             "type": "row"
         },
         {
             "aliasColors": {},
             "bars": false,
             "dashLength": 10,
             "dashes": false,
-            "datasource": null,
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 9,
                 "w": 12,
                 "x": 0,
                 "y": 55
@@ -1004,15 +960,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": false,
             "steppedLine": false,
@@ -1042,61 +998,51 @@
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "Limit memory usage",
                     "refId": "C"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Traefik memory usage",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "format": "bytes",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
-                    "min": null,
                     "show": true
                 },
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
-                    "min": null,
                     "show": false
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         },
         {
             "aliasColors": {},
             "bars": false,
             "dashLength": 10,
             "dashes": false,
-            "datasource": "$Prometheus",
-            "decimals": null,
+            "datasource": {
+                "uid": "$Prometheus"
+            },
             "fill": 1,
             "fillGradient": 0,
             "gridPos": {
                 "h": 9,
                 "w": 12,
                 "x": 12,
                 "y": 55
@@ -1117,15 +1063,15 @@
             "linewidth": 1,
             "links": [],
             "nullPointMode": "null",
             "options": {
                 "alertThreshold": true
             },
             "percentage": false,
-            "pluginVersion": "8.0.3",
+            "pluginVersion": "8.3.3",
             "pointradius": 5,
             "points": false,
             "renderer": "flot",
             "seriesOverrides": [],
             "spaceLength": 10,
             "stack": false,
             "steppedLine": false,
@@ -1155,121 +1101,105 @@
                     "interval": "",
                     "intervalFactor": 1,
                     "legendFormat": "Limit cpu usage",
                     "refId": "C"
                 }
             ],
             "thresholds": [],
-            "timeFrom": null,
             "timeRegions": [],
-            "timeShift": null,
             "title": "Traefik CPU usage",
             "tooltip": {
                 "shared": true,
                 "sort": 0,
                 "value_type": "individual"
             },
             "type": "graph",
             "xaxis": {
-                "buckets": null,
                 "mode": "time",
-                "name": null,
                 "show": true,
                 "values": []
             },
             "yaxes": [
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
-                    "min": null,
                     "show": true
                 },
                 {
                     "format": "short",
-                    "label": null,
                     "logBase": 1,
-                    "max": null,
-                    "min": null,
                     "show": true
                 }
             ],
             "yaxis": {
-                "align": false,
-                "alignLevel": null
+                "align": false
             }
         }
     ],
-    "refresh": "",
-    "schemaVersion": 30,
+    "refresh": "10s",
+    "schemaVersion": 34,
     "style": "dark",
     "tags": [],
     "templating": {
         "list": [
             {
                 "current": {
                     "selected": false,
                     "text": "Prometheus",
                     "value": "Prometheus"
                 },
-                "description": null,
-                "error": null,
                 "hide": 0,
                 "includeAll": false,
                 "label": "Datasource",
                 "multi": false,
                 "name": "Prometheus",
                 "options": [],
                 "query": "prometheus",
                 "queryValue": "",
                 "refresh": 1,
                 "regex": "",
                 "skipUrlSync": false,
                 "type": "datasource"
             },
             {
-                "allValue": null,
                 "current": {
-                    "selected": false,
+                    "selected": true,
                     "text": "dev",
                     "value": "dev"
                 },
-                "datasource": "Prometheus",
-                "definition": "label_values(traefik_config_reloads_total, namespace)",
-                "description": null,
-                "error": null,
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "definition": "label_values(kube_pod_container_info{pod=~\".*traefik.*\"}, namespace)",
                 "hide": 0,
                 "includeAll": false,
                 "label": "Namespace",
                 "multi": false,
                 "name": "namespace",
                 "options": [],
                 "query": {
-                    "query": "label_values(kube_pod_container_info{pod=~\".*traefik.*\", job=\"traefik\"}, namespace)",
-                    "refId": "Prometheus-namespace-Variable-Query"
+                    "query": "label_values(kube_pod_container_info{pod=~\".*traefik.*\"}, namespace)",
+                    "refId": "StandardVariableQuery"
                 },
                 "refresh": 1,
                 "regex": "",
                 "skipUrlSync": false,
                 "sort": 1,
                 "tagValuesQuery": "",
                 "tagsQuery": "",
                 "type": "query",
                 "useTags": false
             },
             {
-                "allValue": null,
                 "current": {
                     "selected": true,
                     "text": "95",
                     "value": "95"
                 },
-                "description": null,
-                "error": null,
                 "hide": 0,
                 "includeAll": false,
                 "label": "Percentiles",
                 "multi": false,
                 "name": "percentiles",
                 "options": [
                     {
@@ -1287,15 +1217,15 @@
                 "queryValue": "",
                 "skipUrlSync": false,
                 "type": "custom"
             }
         ]
     },
     "time": {
-        "from": "now-5m",
+        "from": "now-6h",
         "to": "now"
     },
     "timepicker": {
         "refresh_intervals": [
             "10s",
             "30s",
             "1m",
@@ -1315,9 +1245,10 @@
             "7d",
             "30d"
         ]
     },
     "timezone": "",
     "title": "Traefik",
     "uid": "2p6nlgS7z",
-    "version": 4
+    "version": 1,
+    "weekStart": ""
 }
```

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf` & `nebari-2023.5.1rc1/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/scripts/aws-force-destroy.py` & `nebari-2023.5.1rc1/scripts/aws-force-destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/scripts/aws-force-destroy.sh` & `nebari-2023.5.1rc1/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/scripts/keycloak-export.py` & `nebari-2023.5.1rc1/scripts/keycloak-export.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/conftest.py` & `nebari-2023.5.1rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/test_cli.py` & `nebari-2023.5.1rc1/tests/test_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,81 @@
-import os
 import subprocess
-import typing
-from pathlib import Path
 
 import pytest
 
 from nebari.schema import InitInputs
 from nebari.utils import load_yaml
 
 PROJECT_NAME = "clitest"
 DOMAIN_NAME = "clitest.dev"
 
 
-def run_cli_cmd(command: str, working_dir: typing.Union[str, Path]):
-    """Run the provided CLI command using subprocess."""
-    try:
-        os.chdir(working_dir)
-        subprocess.call(command.split())
-    except subprocess.CalledProcessError:
-        return False
-
-    return True
-
-
 @pytest.mark.parametrize(
     "namespace, auth_provider, ci_provider, ssl_cert_email",
     (
         [None, None, None, None],
         ["prod", "github", "github-actions", "it@acme.org"],
     ),
 )
 def test_nebari_init(tmp_path, namespace, auth_provider, ci_provider, ssl_cert_email):
     """Test `nebari init` CLI command."""
-    command = f"nebari init local --project {PROJECT_NAME} --domain {DOMAIN_NAME} --disable-prompt"
+    command = [
+        "nebari",
+        "init",
+        "local",
+        f"--project={PROJECT_NAME}",
+        f"--domain={DOMAIN_NAME}",
+        "--disable-prompt",
+    ]
 
     default_values = InitInputs()
 
     if namespace:
-        command += f" --namespace {namespace}"
+        command.append(f"--namespace={namespace}")
     else:
         namespace = default_values.namespace
     if auth_provider:
-        command += f" --auth-provider {auth_provider}"
+        command.append(f"--auth-provider={auth_provider}")
     else:
         auth_provider = default_values.auth_provider
     if ci_provider:
-        command += f" --ci-provider {ci_provider}"
+        command.append(f"--ci-provider={ci_provider}")
     else:
         ci_provider = default_values.ci_provider
     if ssl_cert_email:
-        command += f" --ssl-cert-email {ssl_cert_email}"
+        command.append(f"--ssl-cert-email={ssl_cert_email}")
     else:
         ssl_cert_email = default_values.ssl_cert_email
 
-    assert run_cli_cmd(command, tmp_path)
+    subprocess.run(command, cwd=tmp_path, check=True)
 
     config = load_yaml(tmp_path / "nebari-config.yaml")
 
     assert config.get("namespace") == namespace
     assert (
         config.get("security", {}).get("authentication", {}).get("type").lower()
         == auth_provider
     )
     ci_cd = config.get("ci_cd", None)
     if ci_cd:
         assert ci_cd.get("type", {}) == ci_provider
     else:
         assert ci_cd == ci_provider
-        ci_cd = config.get("ci_cd", None)
     acme_email = config.get("certificate", None)
     if acme_email:
         assert acme_email.get("acme_email") == ssl_cert_email
     else:
         assert acme_email == ssl_cert_email
+
+
+def test_python_invocation():
+    def run(command):
+        return subprocess.run(
+            command, check=True, capture_output=True, text=True
+        ).stdout.strip()
+
+    command = ["nebari", "--version"]
+
+    actual = run(["python", "-m", *command])
+    expected = run(command)
+
+    assert actual == expected
```

### Comparing `nebari-2023.4.1a5/tests/test_dependencies.py` & `nebari-2023.5.1rc1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/test_init.py` & `nebari-2023.5.1rc1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/test_render.py` & `nebari-2023.5.1rc1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/test_schema.py` & `nebari-2023.5.1rc1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/test_upgrade.py` & `nebari-2023.5.1rc1/tests/test_upgrade.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,19 @@
 )
 def test_upgrade_4_0(
     old_qhub_config_path_str,
     attempt_fixes,
     expect_upgrade_error,
     tmp_path,
     qhub_users_import_json,
+    monkeypatch,
 ):
+    # Return "y" when asked if you've deleted the Argo CRDs
+    monkeypatch.setattr("builtins.input", lambda: "y")
+
     old_qhub_config_path = Path(__file__).parent / old_qhub_config_path_str
 
     tmp_qhub_config = Path(tmp_path, old_qhub_config_path.name)
     tmp_qhub_config.write_text(old_qhub_config_path.read_text())  # Copy contents to tmp
 
     orig_contents = tmp_qhub_config.read_text()  # Read in initial contents
```

### Comparing `nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2023.5.1rc1/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/scripts/minikube-loadbalancer-ip.py` & `nebari-2023.5.1rc1/tests/scripts/minikube-loadbalancer-ip.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests/vale/styles/vocab.txt` & `nebari-2023.5.1rc1/tests/vale/styles/vocab.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests_deployment/test_dask_gateway.py` & `nebari-2023.5.1rc1/tests_deployment/test_dask_gateway.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,19 +18,23 @@
     return dask_gateway.Gateway(
         address=f"https://{constants.NEBARI_HOSTNAME}/{constants.GATEWAY_ENDPOINT}",
         auth="jupyterhub",
         proxy_address=f"tcp://{constants.NEBARI_HOSTNAME}:8786",
     )
 
 
+@pytest.mark.filterwarnings("ignore::urllib3.exceptions.InsecureRequestWarning")
+@pytest.mark.filterwarnings("ignore::ResourceWarning")
 def test_dask_gateway(dask_gateway_object):
     """This test checks if we're able to connect to dask gateway."""
     assert dask_gateway_object.list_clusters() == []
 
 
+@pytest.mark.filterwarnings("ignore::urllib3.exceptions.InsecureRequestWarning")
+@pytest.mark.filterwarnings("ignore::ResourceWarning")
 def test_dask_gateway_cluster_options(dask_gateway_object):
     """Tests Dask Gateway's cluster options."""
     cluster_options = dask_gateway_object.cluster_options()
     # # dask conda environment is not built in time to be available
     # assert cluster_options.conda_environment == "dask"
     assert cluster_options.profile in {"Small Worker", "Medium Worker"}
     assert cluster_options.environment_vars == {}
```

### Comparing `nebari-2023.4.1a5/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2023.5.1rc1/tests_deployment/test_jupyterhub_ssh.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 
 monkeypatch_ssl_context()
 
 TIMEOUT_SECS = 300
 
 
-@pytest.fixture
+@pytest.fixture(scope="function")
 def paramiko_object():
     """Connects to JupyterHub ssh cluster from outside the cluster."""
     api_token = get_jupyterhub_token("jupyterhub-ssh")
 
     try:
         client = paramiko.SSHClient()
         client.set_missing_host_key_policy(paramiko.AutoAddPolicy)
@@ -56,19 +56,23 @@
         if delimiter not in line:
             output.append(line)
 
     return "".join(output).strip()
 
 
 @pytest.mark.timeout(TIMEOUT_SECS)
+@pytest.mark.filterwarnings("ignore::urllib3.exceptions.InsecureRequestWarning")
+@pytest.mark.filterwarnings("ignore::ResourceWarning")
 def test_simple_jupyterhub_ssh(paramiko_object):
     stdin, stdout, stderr = paramiko_object.exec_command("")
 
 
 @pytest.mark.timeout(TIMEOUT_SECS)
+@pytest.mark.filterwarnings("ignore::urllib3.exceptions.InsecureRequestWarning")
+@pytest.mark.filterwarnings("ignore::ResourceWarning")
 def test_print_jupyterhub_ssh(paramiko_object):
     stdin, stdout, stderr = paramiko_object.exec_command("")
 
     # commands to run and just print the output
     commands_print = [
         "id",
         "env",
@@ -80,14 +84,16 @@
 
     for command in commands_print:
         print(f'COMMAND: "{command}"')
         print(run_command(command, stdin, stdout, stderr))
 
 
 @pytest.mark.timeout(TIMEOUT_SECS)
+@pytest.mark.filterwarnings("ignore::urllib3.exceptions.InsecureRequestWarning")
+@pytest.mark.filterwarnings("ignore::ResourceWarning")
 def test_exact_jupyterhub_ssh(paramiko_object):
     stdin, stdout, stderr = paramiko_object.exec_command("")
 
     # commands to run and exactly match output
     commands_exact = [
         ("id -u", "1000"),
         ("id -g", "100"),
@@ -99,14 +105,16 @@
     ]
 
     for command, output in commands_exact:
         assert output == run_command(command, stdin, stdout, stderr)
 
 
 @pytest.mark.timeout(TIMEOUT_SECS)
+@pytest.mark.filterwarnings("ignore::urllib3.exceptions.InsecureRequestWarning")
+@pytest.mark.filterwarnings("ignore::ResourceWarning")
 def test_contains_jupyterhub_ssh(paramiko_object):
     stdin, stdout, stderr = paramiko_object.exec_command("")
 
     # commands to run and string need to be contained in output
     commands_contain = [
         ("ls -la", ".bashrc"),
         ("cat ~/.bashrc", "Managed by Nebari"),
```

### Comparing `nebari-2023.4.1a5/tests_deployment/utils.py` & `nebari-2023.5.1rc1/tests_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2023.5.1rc1/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests_e2e/package-lock.json` & `nebari-2023.5.1rc1/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests_e2e/cypress/integration/main.js` & `nebari-2023.5.1rc1/tests_e2e/cypress/integration/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -56,15 +56,15 @@
 
             cy.get('input.btn.btn-jupyter')
                 .should('have.attr', 'value', 'Start').click();
 
             // Minimal check that JupyterLab has opened
             cy.get('div#jp-MainLogo', {
                 timeout: 60000
-            }).should('exist').wait(500);
+            }).should('exist').wait(4000);
 
             // Click VS Code Launcher exists
             cy.get('div.jp-LauncherCard[title="VS Code [↗]"]').should('exist');
 
             // Stop my Jupyter server - must do this so PVC can be destroyed on Minikube
             cy.visit('/hub/home');
```

### Comparing `nebari-2023.4.1a5/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2023.5.1rc1/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests_e2e/cypress/plugins/index.js` & `nebari-2023.5.1rc1/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/tests_e2e/cypress/support/index.js` & `nebari-2023.5.1rc1/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/.gitignore` & `nebari-2023.5.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/LICENSE` & `nebari-2023.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/README.md` & `nebari-2023.5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/pyproject.toml` & `nebari-2023.5.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a5/PKG-INFO` & `nebari-2023.5.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari
-Version: 2023.4.1a5
+Version: 2023.5.1rc1
 Summary: A Jupyter and Dask-powered open source data science platform.
 Project-URL: Documentation, https://www.nebari.dev/docs
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
```

