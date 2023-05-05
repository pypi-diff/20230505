# Comparing `tmp/idem-aws-1.7.4.tar.gz` & `tmp/idem-aws-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-aws-1.7.4.tar", last modified: Mon Apr 24 13:10:01 2023, max compression
+gzip compressed data, was "idem-aws-1.7.5.tar", last modified: Fri May  5 18:38:41 2023, max compression
```

## Comparing `idem-aws-1.7.4.tar` & `idem-aws-1.7.5.tar`

### file list

```diff
@@ -1,696 +1,696 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.091292 idem-aws-1.7.4/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-04-24 13:09:47.000000 idem-aws-1.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-24 13:09:47.000000 idem-aws-1.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11051 2023-04-24 13:10:01.091292 idem-aws-1.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9835 2023-04-24 13:09:47.000000 idem-aws-1.7.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.043292 idem-aws-1.7.4/idem_aws/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws/acct/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws/acct/aws/contracts/
--rw-r--r--   0 root         (0) root         (0)     1127 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/acct/aws/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     5506 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/acct/aws/gsuite.py
--rw-r--r--   0 root         (0) root         (0)     1618 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/acct/aws/iam.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/acct/aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws/acct/metadata/
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/acct/metadata/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.043292 idem-aws-1.7.4/idem_aws/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws/autogen/aws/
--rw-r--r--   0 root         (0) root         (0)     7082 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/function.py
--rw-r--r--   0 root         (0) root         (0)     9947 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/init.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/param.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/plugin.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/possible_functions.py
--rw-r--r--   0 root         (0) root         (0)     3870 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/resource.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws/autogen/aws/tag/
--rw-r--r--   0 root         (0) root         (0)     3401 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/tag/plugin.py
--rw-r--r--   0 root         (0) root         (0)     4865 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/tag/template.py
--rw-r--r--   0 root         (0) root         (0)    15883 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/autogen/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/utils/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/autogen/aws/utils/template.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/esm/
--rw-r--r--   0 root         (0) root         (0)     8692 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/esm/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/esm/contracts/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/esm/contracts/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.043292 idem-aws-1.7.4/idem_aws/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/acm/
--rw-r--r--   0 root         (0) root         (0)     2000 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/acm/certificate_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)     5430 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigateway/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)     3276 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)     3192 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/application_autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/arn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)     3034 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     4661 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/backup/backup_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)     4105 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/budgets/budget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)     2285 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)     4007 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/cloudfront/cache_policy.py
--rw-r--r--   0 root         (0) root         (0)     2697 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/cloudfront/origin_request_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)     3012 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/cloudwatch/log_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/config/
--rw-r--r--   0 root         (0) root         (0)     4538 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/config/configuration_aggregator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)     6138 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7293 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     4887 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/docdb/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.051292 idem-aws-1.7.4/idem_aws/exec/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)     2434 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/dynamodb/table.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/dynamodb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)     8697 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/availability_zones.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/flow_log.py
--rw-r--r--   0 root         (0) root         (0)    22002 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/instance.py
--rw-r--r--   0 root         (0) root         (0)     3299 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)     7293 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)     8395 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)     4680 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)     5836 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/route.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     3265 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/route_table_association.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/security_group.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4295 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)     8595 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)     4471 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)     4459 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_peering_connection.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)     5183 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ecr/image.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ecr/lifecycle_policy.py
--rw-r--r--   0 root         (0) root         (0)     5504 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ecr/repository.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ecr/repository_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/eks/
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/eks/cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)     2934 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/elasticache/replication_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/elb/
--rw-r--r--   0 root         (0) root         (0)     3023 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/elb/elb_hosted_zone_id.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/elb/load_balancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)     3296 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     4861 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/es/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/es/elasticsearch_domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/events/
--rw-r--r--   0 root         (0) root         (0)     5682 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/events/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)     2423 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/guardduty/detector.py
--rw-r--r--   0 root         (0) root         (0)     5618 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/guardduty/member.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/guardduty/organization_admin_account.py
--rw-r--r--   0 root         (0) root         (0)     8637 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/guardduty/organization_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/iam/
--rw-r--r--   0 root         (0) root         (0)     9324 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/access_key.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     2099 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/group_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     4749 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/instance_profile.py
--rw-r--r--   0 root         (0) root         (0)     7709 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/open_id_connect_provider.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)     6957 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)     9723 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/role.py
--rw-r--r--   0 root         (0) root         (0)     1218 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/iam/user_policy_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)     2919 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/kinesis/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/kms/
--rw-r--r--   0 root         (0) root         (0)     3031 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/kms/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)     4863 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)     5632 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/lambda_aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)     7388 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6854 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/neptune/db_parameter_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)     4486 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/organizations/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.055292 idem-aws-1.7.4/idem_aws/exec/aws/rds/
--rw-r--r--   0 root         (0) root         (0)     5996 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/rds/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5001 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/rds/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     5971 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/rds/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6287 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/rds/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/rds/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/rds/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/route53/
--rw-r--r--   0 root         (0) root         (0)     5251 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/route53/hosted_zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/s3/
--rw-r--r--   0 root         (0) root         (0)     2659 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_website.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ses/domain_identity.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/ses/identity_notification_topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)     4342 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/sesv2/event_destination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/sns/
--rw-r--r--   0 root         (0) root         (0)     3682 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/sns/subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)     4686 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/sqs/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/sts/
--rw-r--r--   0 root         (0) root         (0)     5261 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/sts/assume_role.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/sts/caller_identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     4859 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/wafv2/ip_set.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/aws/wafv2/regex_pattern_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/exec/boto3/
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/exec/boto3/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.043292 idem-aws-1.7.4/idem_aws/reconcile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/reconcile/pending/
--rw-r--r--   0 root         (0) root         (0)     1004 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/reconcile/pending/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.043292 idem-aws-1.7.4/idem_aws/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/acm/
--rw-r--r--   0 root         (0) root         (0)    28336 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/acm/certificate_manager.py
--rw-r--r--   0 root         (0) root         (0)    11133 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/acm/certificate_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)     9915 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11767 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)    19520 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)    15779 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)    13752 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)    12480 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)    12155 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     9586 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)    13732 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)    13857 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigateway/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)    15354 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)    16244 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)    15119 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)    22419 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)    13754 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/route.py
--rw-r--r--   0 root         (0) root         (0)    16655 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/stage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)    31323 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)    45295 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/application_autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)    78777 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/autoscaling/auto_scaling_group.py
--rw-r--r--   0 root         (0) root         (0)    32523 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/autoscaling/launch_configuration.py
--rw-r--r--   0 root         (0) root         (0)    54633 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/autoscaling/scaling_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     8985 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/backup/backup_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)    25523 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/budgets/budget.py
--rw-r--r--   0 root         (0) root         (0)    16117 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/budgets/budget_action.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/caller_identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.059292 idem-aws-1.7.4/idem_aws/states/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)    32414 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)    24459 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudfront/cache_policy.py
--rw-r--r--   0 root         (0) root         (0)   116074 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)    15501 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudfront/origin_request_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/cloudtrail/
--rw-r--r--   0 root         (0) root         (0)    37423 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudtrail/trail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)    11420 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudwatch/log_group.py
--rw-r--r--   0 root         (0) root         (0)    36077 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudwatch/metric_alarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)     8723 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/cloudwatchlogs/resource_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/config/
--rwxr-xr-x   0 root         (0) root         (0)    11422 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/config/config_recorder.py
--rwxr-xr-x   0 root         (0) root         (0)     9512 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/config/config_recorder_status.py
--rw-r--r--   0 root         (0) root         (0)    10463 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/config/configuration_aggregator.py
--rwxr-xr-x   0 root         (0) root         (0)    12062 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/config/delivery_channel.py
--rw-r--r--   0 root         (0) root         (0)    21665 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/config/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)    18428 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/costexplorer/anomaly_monitor.py
--rw-r--r--   0 root         (0) root         (0)    10521 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/costexplorer/anomaly_subscription.py
--rw-r--r--   0 root         (0) root         (0)    28397 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/costexplorer/cost_category.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)    28355 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    12967 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    11755 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/docdb/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)    36228 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/dynamodb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.063292 idem-aws-1.7.4/idem_aws/states/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)    22039 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)    15794 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/dhcp_option.py
--rw-r--r--   0 root         (0) root         (0)     9508 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/dhcp_option_association.py
--rw-r--r--   0 root         (0) root         (0)    13002 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)    12633 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/flow_log.py
--rw-r--r--   0 root         (0) root         (0)    40732 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/instance.py
--rw-r--r--   0 root         (0) root         (0)    12429 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     9711 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)    73136 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)    17418 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/nat_gateway.py
--rw-r--r--   0 root         (0) root         (0)    12093 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)    10929 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)    14835 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/route.py
--rw-r--r--   0 root         (0) root         (0)    15623 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     8933 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/route_table_association.py
--rw-r--r--   0 root         (0) root         (0)    12947 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/security_group.py
--rw-r--r--   0 root         (0) root         (0)    17979 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)    10496 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)    36976 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    20046 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)    17765 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/transit_gateway.py
--rw-r--r--   0 root         (0) root         (0)    16953 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py
--rw-r--r--   0 root         (0) root         (0)    15314 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)    20607 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)    19294 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    14516 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_peering_connection.py
--rw-r--r--   0 root         (0) root         (0)     9205 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py
--rw-r--r--   0 root         (0) root         (0)     9851 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_peering_connection_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)    11576 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ecr/lifecycle_policy.py
--rw-r--r--   0 root         (0) root         (0)    13319 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ecr/repository.py
--rw-r--r--   0 root         (0) root         (0)    11690 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ecr/repository_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/efs/
--rw-r--r--   0 root         (0) root         (0)    25301 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/efs/file_system.py
--rw-r--r--   0 root         (0) root         (0)    22100 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/efs/mount_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/eks/
--rw-r--r--   0 root         (0) root         (0)    17811 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/eks/addon.py
--rw-r--r--   0 root         (0) root         (0)    29585 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/eks/cluster.py
--rw-r--r--   0 root         (0) root         (0)    17220 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/eks/fargate_profile.py
--rw-r--r--   0 root         (0) root         (0)    29516 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/eks/nodegroup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)    16170 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/elasticache/cache_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    13492 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/elasticache/cache_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)    51005 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/elasticache/replication_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/elb/
--rw-r--r--   0 root         (0) root         (0)    19828 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/elb/load_balancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)    32920 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)    24159 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)    30475 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/es/
--rw-r--r--   0 root         (0) root         (0)    36336 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/es/elasticsearch_domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/events/
--rw-r--r--   0 root         (0) root         (0)    45263 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/events/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)    15458 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/guardduty/detector.py
--rw-r--r--   0 root         (0) root         (0)     9782 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/guardduty/member.py
--rw-r--r--   0 root         (0) root         (0)     8751 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/guardduty/organization_admin_account.py
--rw-r--r--   0 root         (0) root         (0)     8981 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/guardduty/organization_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/iam/
--rw-r--r--   0 root         (0) root         (0)     9717 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/access_key.py
--rw-r--r--   0 root         (0) root         (0)     8236 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     8164 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     8426 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/group_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    14295 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/instance_profile.py
--rw-r--r--   0 root         (0) root         (0)    18379 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/open_id_connect_provider.py
--rw-r--r--   0 root         (0) root         (0)    12320 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)    14613 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)    22432 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/role.py
--rw-r--r--   0 root         (0) root         (0)    14538 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/role_policy.py
--rw-r--r--   0 root         (0) root         (0)    10279 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/role_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    15245 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/service_linked_role.py
--rw-r--r--   0 root         (0) root         (0)    15326 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)    14080 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/user_policy.py
--rw-r--r--   0 root         (0) root         (0)    10805 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/user_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)    12784 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/iam/user_ssh_key.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)    24104 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/kinesis/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/kms/
--rw-r--r--   0 root         (0) root         (0)    10460 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/kms/alias.py
--rw-r--r--   0 root         (0) root         (0)    22629 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/kms/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)    27963 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function.py
--rw-r--r--   0 root         (0) root         (0)    11651 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)    13745 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function_permission.py
--rw-r--r--   0 root         (0) root         (0)    10018 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.067292 idem-aws-1.7.4/idem_aws/states/aws/logs/
--rw-r--r--   0 root         (0) root         (0)    11749 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/logs/subscription_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)    32988 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/neptune/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    13936 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    37556 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)    12467 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/neptune/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    14288 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/neptune/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)    17151 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/organizations/organization.py
--rw-r--r--   0 root         (0) root         (0)    14047 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/organizations/organization_unit.py
--rw-r--r--   0 root         (0) root         (0)    13651 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/organizations/policy.py
--rw-r--r--   0 root         (0) root         (0)    10853 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/organizations/policy_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/rds/
--rw-r--r--   0 root         (0) root         (0)    62077 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/rds/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)    14695 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/rds/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    39434 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/rds/db_instance.py
--rw-r--r--   0 root         (0) root         (0)    13857 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/rds/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    14036 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/rds/db_subnet_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/recursive_contracts/allow_sync_sls_name_and_name_tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/route53/
--rw-r--r--   0 root         (0) root         (0)    19436 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/route53/hosted_zone.py
--rw-r--r--   0 root         (0) root         (0)    14158 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/route53/hosted_zone_association.py
--rw-r--r--   0 root         (0) root         (0)    12020 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/route53/resource_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/s3/
--rw-r--r--   0 root         (0) root         (0)    19835 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)    12547 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)    26660 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)    14837 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)    17615 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)    11689 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)    27930 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)    10328 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)    22351 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_website.py
--rw-r--r--   0 root         (0) root         (0)    12854 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/s3/public_access_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     6158 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ses/domain_identity.py
--rw-r--r--   0 root         (0) root         (0)    10385 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/ses/identity_notification_topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)    14259 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/sesv2/event_destination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/sns/
--rw-r--r--   0 root         (0) root         (0)    11183 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/sns/subscription.py
--rw-r--r--   0 root         (0) root         (0)    13035 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/sns/topic.py
--rw-r--r--   0 root         (0) root         (0)     8472 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/sns/topic_policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)    24692 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/sqs/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.071292 idem-aws-1.7.4/idem_aws/states/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     9933 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/wafv2/associate_web_acl.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/wafv2/ip_set.py
--rw-r--r--   0 root         (0) root         (0)    12255 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/wafv2/regex_pattern_set.py
--rw-r--r--   0 root         (0) root         (0)   268538 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/states/aws/wafv2/web_acl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/acct/
--rw-r--r--   0 root         (0) root         (0)     1393 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acct/assume_role.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/acct/contracts/
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acct/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acct/esm.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acct/init.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acct/key_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/acm/
--rw-r--r--   0 root         (0) root         (0)     2485 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acm/certificate_validation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acm/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2625 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/acm/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/
--rw-r--r--   0 root         (0) root         (0)     3883 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/base_path_mapping.py
--rw-r--r--   0 root         (0) root         (0)     3343 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/deployment.py
--rw-r--r--   0 root         (0) root         (0)     8767 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     4535 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/integration.py
--rw-r--r--   0 root         (0) root         (0)     5000 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/integration_response.py
--rw-r--r--   0 root         (0) root         (0)     4226 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/method.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/method_response.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/resource.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/rest_api.py
--rw-r--r--   0 root         (0) root         (0)     4417 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/stage.py
--rw-r--r--   0 root         (0) root         (0)     2203 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigateway/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/
--rw-r--r--   0 root         (0) root         (0)     5671 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/api.py
--rw-r--r--   0 root         (0) root         (0)     5125 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/authorizer.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/domain_name.py
--rw-r--r--   0 root         (0) root         (0)     5187 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/integration.py
--rw-r--r--   0 root         (0) root         (0)     4793 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/route.py
--rw-r--r--   0 root         (0) root         (0)     4061 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/stage.py
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/application_autoscaling/
--rw-r--r--   0 root         (0) root         (0)     2724 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/application_autoscaling/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/application_autoscaling/scalable_target.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/application_autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     4099 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/arn_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/
--rw-r--r--   0 root         (0) root         (0)     5561 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py
--rw-r--r--   0 root         (0) root         (0)     4257 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3367 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/scaling_policy.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/tag.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/b64.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/backup/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/backup/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/backup/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/budgets/
--rw-r--r--   0 root         (0) root         (0)     5249 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/budgets/budget.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/budgets/budget_action.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/budgets/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/cloudformation/
--rw-r--r--   0 root         (0) root         (0)    18904 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudformation/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/
--rw-r--r--   0 root         (0) root         (0)     6468 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/cloudfront_utils.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7502 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/distribution.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/distribution_utils.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.075292 idem-aws-1.7.4/idem_aws/tool/aws/cloudtrail/
--rw-r--r--   0 root         (0) root         (0)     3966 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudtrail/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    13076 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudtrail/trail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/
--rw-r--r--   0 root         (0) root         (0)     3540 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)      807 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/log_group.py
--rw-r--r--   0 root         (0) root         (0)     4464 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/metric_alarm.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/cloudwatchlogs/
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/config/
--rw-r--r--   0 root         (0) root         (0)     1511 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/config/config_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     4483 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/config/delivery_channel.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/config/rule.py
--rw-r--r--   0 root         (0) root         (0)     2434 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/config/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/
--rw-r--r--   0 root         (0) root         (0)     1024 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/anomaly_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/anomaly_subscription.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/cost_category.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/docdb/
--rw-r--r--   0 root         (0) root         (0)    12556 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/docdb/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     6638 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/docdb/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/docdb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/dynamodb/
--rw-r--r--   0 root         (0) root         (0)    15451 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/dynamodb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/ec2/
--rw-r--r--   0 root         (0) root         (0)     3051 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/ami.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/availability_zones.py
--rw-r--r--   0 root         (0) root         (0)    37442 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/elastic_ip.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/flow_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.079292 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/
--rw-r--r--   0 root         (0) root         (0)     1280 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/data.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/key_pair.py
--rw-r--r--   0 root         (0) root         (0)    19910 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/
--rw-r--r--   0 root         (0) root         (0)     4440 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/bootstrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/contracts/
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py
--rw-r--r--   0 root         (0) root         (0)     8226 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/init.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/kernel_id.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py
--rw-r--r--   0 root         (0) root         (0)     4123 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/placement.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/running.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/tags.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/user_data.py
--rw-r--r--   0 root         (0) root         (0)     4843 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/internet_gateway.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/key_pair.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/launch_template.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/network_interface.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/placement_group.py
--rw-r--r--   0 root         (0) root         (0)    12208 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/route_table.py
--rw-r--r--   0 root         (0) root         (0)     3924 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/security_group_rule.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/spot_instance_request.py
--rw-r--r--   0 root         (0) root         (0)    14415 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/subnet.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/tag.py
--rw-r--r--   0 root         (0) root         (0)     3821 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/transit_gateway.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/volume.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/vpc.py
--rw-r--r--   0 root         (0) root         (0)     8498 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/vpc_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    10282 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/ecr/
--rw-r--r--   0 root         (0) root         (0)     4995 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ecr/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ecr/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/efs/
--rw-r--r--   0 root         (0) root         (0)     2368 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/efs/file_system_utils.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/efs/mount_target_utils.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/efs/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/eks/
--rw-r--r--   0 root         (0) root         (0)     4881 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/eks/addon.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/eks/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5220 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/eks/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     4559 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/eks/eks_utils.py
--rw-r--r--   0 root         (0) root         (0)     7710 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/eks/nodegroup.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/eks/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/elasticache/
--rw-r--r--   0 root         (0) root         (0)     9303 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elasticache/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    20325 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elasticache/elasticache_utils.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elasticache/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/elb/
--rw-r--r--   0 root         (0) root         (0)     1957 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elb/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    19196 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elb/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     2429 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elb/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/elbv2/
--rw-r--r--   0 root         (0) root         (0)     7683 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elbv2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    10904 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elbv2/listener.py
--rw-r--r--   0 root         (0) root         (0)    10107 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elbv2/load_balancer.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elbv2/tag.py
--rw-r--r--   0 root         (0) root         (0)    10958 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/elbv2/target_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/es/
--rw-r--r--   0 root         (0) root         (0)     9741 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/es/elasticsearch_domain.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/es/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/events/
--rw-r--r--   0 root         (0) root         (0)     1707 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/events/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     5958 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/events/rule.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/events/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/guardduty/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/guardduty/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/guardduty/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7045 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/guardduty/detector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/iam/
--rw-r--r--   0 root         (0) root         (0)    12738 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/group.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/group_membership.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/password_policy.py
--rw-r--r--   0 root         (0) root         (0)     7466 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/policy.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/role_policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/service_linked_role.py
--rw-r--r--   0 root         (0) root         (0)     3720 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/user.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/iam/user_ssh_key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.083292 idem-aws-1.7.4/idem_aws/tool/aws/kinesis/
--rw-r--r--   0 root         (0) root         (0)     1976 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/kinesis/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    21390 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/kinesis/stream.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/kinesis/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/kms/
--rw-r--r--   0 root         (0) root         (0)      999 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/kms/alias.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/kms/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/kms/key.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/kms/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/
--rw-r--r--   0 root         (0) root         (0)     3194 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    16057 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function_permission.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/init.py
--rw-r--r--   0 root         (0) root         (0)     2689 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/logs/
--rw-r--r--   0 root         (0) root         (0)     1336 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/logs/subscription_filter_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/neptune/
--rw-r--r--   0 root         (0) root         (0)     8991 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/neptune/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    12251 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_cluster.py
--rw-r--r--   0 root         (0) root         (0)     6385 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)    11654 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_instance.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_parameter_group.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_subnet_group.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/neptune/tag.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/network_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/organizations/
--rw-r--r--   0 root         (0) root         (0)     1795 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/organizations/account.py
--rw-r--r--   0 root         (0) root         (0)     4764 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/organizations/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/organizations/policy_attachment.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/organizations/tag.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/rds/
--rw-r--r--   0 root         (0) root         (0)    12718 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/rds/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/rds/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/route53/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/route53/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/route53/hosted_zone_association.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/route53/hosted_zone_utils.py
--rw-r--r--   0 root         (0) root         (0)     7422 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/route53/resource_record_utils.py
--rw-r--r--   0 root         (0) root         (0)     2663 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/route53/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/s3/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_acl.py
--rw-r--r--   0 root         (0) root         (0)     7925 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)     7403 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_logging.py
--rw-r--r--   0 root         (0) root         (0)     2584 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_website.py
--rw-r--r--   0 root         (0) root         (0)     9894 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3373 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/s3/s3_utils.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/search_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/ses/
--rw-r--r--   0 root         (0) root         (0)     1214 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/ses/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/sesv2/
--rw-r--r--   0 root         (0) root         (0)      563 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/sesv2/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/sns/
--rw-r--r--   0 root         (0) root         (0)     3617 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/sns/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     7581 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/sns/sns_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/sqs/
--rw-r--r--   0 root         (0) root         (0)     6482 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/sqs/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     5455 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/sqs/queue_utils.py
--rw-r--r--   0 root         (0) root         (0)     3760 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/state_utils.py
--rw-r--r--   0 root         (0) root         (0)      526 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/string_utils.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/tag_utils.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.087292 idem-aws-1.7.4/idem_aws/tool/aws/wafv2/
--rw-r--r--   0 root         (0) root         (0)     6843 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/wafv2/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     3076 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/wafv2/ip_set_utils.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/wafv2/regex_pattern_set.py
--rw-r--r--   0 root         (0) root         (0)     3822 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/wafv2/tag.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/wafv2/web_acl.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/aws/waiter_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.091292 idem-aws-1.7.4/idem_aws/tool/boto3/
--rw-r--r--   0 root         (0) root         (0)     5000 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/boto3/client.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/boto3/custom_waiter.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/boto3/exception.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/boto3/region.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/boto3/resolve.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/boto3/resource.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/boto3/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.091292 idem-aws-1.7.4/idem_aws/tool/heist/
--rw-r--r--   0 root         (0) root         (0)      906 2023-04-24 13:09:47.000000 idem-aws-1.7.4/idem_aws/tool/heist/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-24 13:10:00.000000 idem-aws-1.7.4/idem_aws/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:10:01.047292 idem-aws-1.7.4/idem_aws.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11051 2023-04-24 13:10:00.000000 idem-aws-1.7.4/idem_aws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22825 2023-04-24 13:10:01.000000 idem-aws-1.7.4/idem_aws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:10:00.000000 idem-aws-1.7.4/idem_aws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-24 13:10:00.000000 idem-aws-1.7.4/idem_aws.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-24 13:10:00.000000 idem-aws-1.7.4/idem_aws.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      365 2023-04-24 13:09:47.000000 idem-aws-1.7.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 13:10:01.091292 idem-aws-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3136 2023-04-24 13:09:47.000000 idem-aws-1.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.895220 idem-aws-1.7.5/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-05-05 18:38:25.000000 idem-aws-1.7.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-05 18:38:25.000000 idem-aws-1.7.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11051 2023-05-05 18:38:41.895220 idem-aws-1.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.839216 idem-aws-1.7.5/idem_aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.829215 idem-aws-1.7.5/idem_aws/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/acct/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/acct/aws/contracts/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/gsuite.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/iam.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/acct/metadata/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/acct/metadata/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.829215 idem-aws-1.7.5/idem_aws/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.840216 idem-aws-1.7.5/idem_aws/autogen/aws/
+-rw-r--r--   0 root         (0) root         (0)     7082 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/function.py
+-rw-r--r--   0 root         (0) root         (0)     9947 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/init.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/param.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/plugin.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/possible_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3870 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/resource.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/autogen/aws/tag/
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/tag/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/tag/template.py
+-rw-r--r--   0 root         (0) root         (0)    15883 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/autogen/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/utils/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/autogen/aws/utils/template.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/esm/
+-rw-r--r--   0 root         (0) root         (0)     8692 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/esm/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/esm/contracts/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/esm/contracts/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.832215 idem-aws-1.7.5/idem_aws/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/exec/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.841216 idem-aws-1.7.5/idem_aws/exec/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/acm/certificate_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.842216 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigateway/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)     3276 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/arn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/backup/backup_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/budgets/budget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.843216 idem-aws-1.7.5/idem_aws/exec/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/cache_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/origin_request_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatch/log_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/config/
+-rw-r--r--   0 root         (0) root         (0)     4538 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/config/configuration_aggregator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)     6138 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.844216 idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/table.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.847216 idem-aws-1.7.5/idem_aws/exec/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)     8697 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/availability_zones.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/flow_log.py
+-rw-r--r--   0 root         (0) root         (0)    22002 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)     7293 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)     8395 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/route.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     3265 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table_association.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)     8595 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.847216 idem-aws-1.7.5/idem_aws/exec/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)     5183 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/image.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/lifecycle_policy.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.847216 idem-aws-1.7.5/idem_aws/exec/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/eks/cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elasticache/replication_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elb/elb_hosted_zone_id.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elb/load_balancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)     3296 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/es/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/es/elasticsearch_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.848216 idem-aws-1.7.5/idem_aws/exec/aws/events/
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/events/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.849216 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/detector.py
+-rw-r--r--   0 root         (0) root         (0)     5618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/member.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_admin_account.py
+-rw-r--r--   0 root         (0) root         (0)     8637 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)     9324 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/access_key.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/group_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/instance_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7709 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/open_id_connect_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/role.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/iam/user_policy_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)     2919 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/kinesis/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/kms/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)     5632 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.850216 idem-aws-1.7.5/idem_aws/exec/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)     7388 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     6621 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_parameter_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.851216 idem-aws-1.7.5/idem_aws/exec/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)     4486 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/organizations/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.851216 idem-aws-1.7.5/idem_aws/exec/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6287 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/rds/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.851216 idem-aws-1.7.5/idem_aws/exec/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/route53/hosted_zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_website.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ses/domain_identity.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/ses/identity_notification_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)     4342 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sesv2/event_destination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sns/subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)     4686 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sqs/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.852217 idem-aws-1.7.5/idem_aws/exec/aws/sts/
+-rw-r--r--   0 root         (0) root         (0)     5261 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sts/assume_role.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/sts/caller_identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/exec/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/wafv2/ip_set.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/aws/wafv2/regex_pattern_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/exec/boto3/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/exec/boto3/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.832215 idem-aws-1.7.5/idem_aws/reconcile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/reconcile/pending/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/reconcile/pending/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.832215 idem-aws-1.7.5/idem_aws/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/states/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.853217 idem-aws-1.7.5/idem_aws/states/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)    28336 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11133 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.854217 idem-aws-1.7.5/idem_aws/states/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)    10257 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)    19520 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)    15779 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)    13752 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)    12951 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     9866 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)    13857 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigateway/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.855217 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)    15354 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)    16244 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)    15119 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)    22693 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)    14022 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/route.py
+-rw-r--r--   0 root         (0) root         (0)    16913 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.855217 idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)    31855 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)    45934 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)    78777 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/auto_scaling_group.py
+-rw-r--r--   0 root         (0) root         (0)    32523 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/launch_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    54968 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/autoscaling/scaling_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     8985 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/backup/backup_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)    25523 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/budgets/budget.py
+-rw-r--r--   0 root         (0) root         (0)    16456 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/budgets/budget_action.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/caller_identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.856217 idem-aws-1.7.5/idem_aws/states/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)    32414 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)    24459 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/cache_policy.py
+-rw-r--r--   0 root         (0) root         (0)   116104 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)    15501 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudfront/origin_request_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudtrail/
+-rw-r--r--   0 root         (0) root         (0)    37423 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudtrail/trail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)    11420 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/log_group.py
+-rw-r--r--   0 root         (0) root         (0)    36077 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/metric_alarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.857217 idem-aws-1.7.5/idem_aws/states/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)     8723 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/cloudwatchlogs/resource_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.858217 idem-aws-1.7.5/idem_aws/states/aws/config/
+-rwxr-xr-x   0 root         (0) root         (0)    11422 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder.py
+-rwxr-xr-x   0 root         (0) root         (0)     9512 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder_status.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/configuration_aggregator.py
+-rwxr-xr-x   0 root         (0) root         (0)    12062 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/delivery_channel.py
+-rw-r--r--   0 root         (0) root         (0)    21665 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/config/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.858217 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)    18654 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    28397 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/costexplorer/cost_category.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.858217 idem-aws-1.7.5/idem_aws/states/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)    28355 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    11755 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/docdb/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.859217 idem-aws-1.7.5/idem_aws/states/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)    36228 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/dynamodb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.862217 idem-aws-1.7.5/idem_aws/states/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)    22039 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)    15794 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option.py
+-rw-r--r--   0 root         (0) root         (0)    10017 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option_association.py
+-rw-r--r--   0 root         (0) root         (0)    13002 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)    12633 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/flow_log.py
+-rw-r--r--   0 root         (0) root         (0)    40732 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/instance.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     9711 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)    73136 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)    17418 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/nat_gateway.py
+-rw-r--r--   0 root         (0) root         (0)    12093 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)    14835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/route.py
+-rw-r--r--   0 root         (0) root         (0)    15623 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     8933 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table_association.py
+-rw-r--r--   0 root         (0) root         (0)    12947 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group.py
+-rw-r--r--   0 root         (0) root         (0)    17979 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)    10513 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    36976 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    20046 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)    17765 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway.py
+-rw-r--r--   0 root         (0) root         (0)    16953 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    15331 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)    20607 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)    19294 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    14516 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection.py
+-rw-r--r--   0 root         (0) root         (0)     9225 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py
+-rw-r--r--   0 root         (0) root         (0)     9871 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.862217 idem-aws-1.7.5/idem_aws/states/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)    11586 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ecr/lifecycle_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13319 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ecr/repository.py
+-rw-r--r--   0 root         (0) root         (0)    11707 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ecr/repository_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.863217 idem-aws-1.7.5/idem_aws/states/aws/efs/
+-rw-r--r--   0 root         (0) root         (0)    25301 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/efs/file_system.py
+-rw-r--r--   0 root         (0) root         (0)    22090 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/efs/mount_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.863217 idem-aws-1.7.5/idem_aws/states/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)    18084 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/addon.py
+-rw-r--r--   0 root         (0) root         (0)    29585 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    17678 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/fargate_profile.py
+-rw-r--r--   0 root         (0) root         (0)    29787 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/eks/nodegroup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.863217 idem-aws-1.7.5/idem_aws/states/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)    51005 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elasticache/replication_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)    19828 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elb/load_balancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)    32920 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)    24159 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)    30475 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/es/
+-rw-r--r--   0 root         (0) root         (0)    36336 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/es/elasticsearch_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.864217 idem-aws-1.7.5/idem_aws/states/aws/events/
+-rw-r--r--   0 root         (0) root         (0)    45263 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/events/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.865218 idem-aws-1.7.5/idem_aws/states/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)    15458 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/detector.py
+-rw-r--r--   0 root         (0) root         (0)    10351 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/member.py
+-rw-r--r--   0 root         (0) root         (0)     8768 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_admin_account.py
+-rw-r--r--   0 root         (0) root         (0)     8981 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.866218 idem-aws-1.7.5/idem_aws/states/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/access_key.py
+-rw-r--r--   0 root         (0) root         (0)     8246 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     8179 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     8776 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/group_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    14496 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/instance_profile.py
+-rw-r--r--   0 root         (0) root         (0)    18389 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/open_id_connect_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12320 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)    14613 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)    22432 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/role.py
+-rw-r--r--   0 root         (0) root         (0)    14538 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    15633 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/service_linked_role.py
+-rw-r--r--   0 root         (0) root         (0)    15522 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)    14080 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11044 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)    13341 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/iam/user_ssh_key.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.866218 idem-aws-1.7.5/idem_aws/states/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)    24114 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/kinesis/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.867218 idem-aws-1.7.5/idem_aws/states/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)    10460 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/kms/alias.py
+-rw-r--r--   0 root         (0) root         (0)    22629 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/kms/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.867218 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)    27963 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function.py
+-rw-r--r--   0 root         (0) root         (0)    11651 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)    14029 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_permission.py
+-rw-r--r--   0 root         (0) root         (0)    10018 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.867218 idem-aws-1.7.5/idem_aws/states/aws/logs/
+-rw-r--r--   0 root         (0) root         (0)    12064 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/logs/subscription_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.868218 idem-aws-1.7.5/idem_aws/states/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)    32988 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    37556 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)    12467 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    14288 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/neptune/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.868218 idem-aws-1.7.5/idem_aws/states/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)    17382 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/organization.py
+-rw-r--r--   0 root         (0) root         (0)    14288 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/organization_unit.py
+-rw-r--r--   0 root         (0) root         (0)    13661 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/policy.py
+-rw-r--r--   0 root         (0) root         (0)    11399 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/organizations/policy_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.869218 idem-aws-1.7.5/idem_aws/states/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)    62077 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    14695 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    39434 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    14036 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/rds/db_subnet_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.869218 idem-aws-1.7.5/idem_aws/states/aws/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/recursive_contracts/allow_sync_sls_name_and_name_tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.870218 idem-aws-1.7.5/idem_aws/states/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)    19436 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone.py
+-rw-r--r--   0 root         (0) root         (0)    14158 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone_association.py
+-rw-r--r--   0 root         (0) root         (0)    12020 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/route53/resource_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)    19835 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)    12547 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)    26660 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)    14837 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)    17615 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)    11956 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)    27930 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)    10328 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)    22433 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_website.py
+-rw-r--r--   0 root         (0) root         (0)    12854 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/s3/public_access_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     6158 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ses/domain_identity.py
+-rw-r--r--   0 root         (0) root         (0)    10385 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/ses/identity_notification_topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)    14618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sesv2/event_destination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)    11622 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sns/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    13240 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sns/topic.py
+-rw-r--r--   0 root         (0) root         (0)     8684 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sns/topic_policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.871218 idem-aws-1.7.5/idem_aws/states/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)    24692 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/sqs/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.872218 idem-aws-1.7.5/idem_aws/states/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     9933 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/associate_web_acl.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/ip_set.py
+-rw-r--r--   0 root         (0) root         (0)    12255 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/regex_pattern_set.py
+-rw-r--r--   0 root         (0) root         (0)   268538 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/states/aws/wafv2/web_acl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.838215 idem-aws-1.7.5/idem_aws/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/acct/
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/assume_role.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/acct/contracts/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/esm.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/init.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acct/key_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.874218 idem-aws-1.7.5/idem_aws/tool/aws/acm/
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acm/certificate_validation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5339 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acm/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/acm/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.876218 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/base_path_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration.py
+-rw-r--r--   0 root         (0) root         (0)     5000 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration_response.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method_response.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/resource.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/rest_api.py
+-rw-r--r--   0 root         (0) root         (0)     4417 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/stage.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigateway/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.876218 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/api.py
+-rw-r--r--   0 root         (0) root         (0)     5125 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/authorizer.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     5187 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/integration.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/route.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/stage.py
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.876218 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scalable_target.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/arn_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)     5561 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3367 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/scaling_policy.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/tag.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/b64.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/backup/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/backup/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/backup/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/budgets/
+-rw-r--r--   0 root         (0) root         (0)     5249 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget_action.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/budgets/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.877218 idem-aws-1.7.5/idem_aws/tool/aws/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)    18904 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudformation/stack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.878219 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/
+-rw-r--r--   0 root         (0) root         (0)     6468 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/cloudfront_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.878219 idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    13076 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/trail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/log_group.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/metric_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatchlogs/
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/config/
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/config_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     4483 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/delivery_channel.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/rule.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/config/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.879219 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/cost_category.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.880219 idem-aws-1.7.5/idem_aws/tool/aws/docdb/
+-rw-r--r--   0 root         (0) root         (0)    12556 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/docdb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.880219 idem-aws-1.7.5/idem_aws/tool/aws/dynamodb/
+-rw-r--r--   0 root         (0) root         (0)    15451 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/dynamodb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.882219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/
+-rw-r--r--   0 root         (0) root         (0)     3051 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/ami.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/availability_zones.py
+-rw-r--r--   0 root         (0) root         (0)    37442 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/elastic_ip.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/flow_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.882219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/data.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)    19910 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.884219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/bootstrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.884219 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/contracts/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/init.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/kernel_id.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/placement.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/running.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/user_data.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/internet_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/key_pair.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/launch_template.py
+-rw-r--r--   0 root         (0) root         (0)     3948 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/network_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/placement_group.py
+-rw-r--r--   0 root         (0) root         (0)    12208 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/route_table.py
+-rw-r--r--   0 root         (0) root         (0)     3924 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/security_group_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/spot_instance_request.py
+-rw-r--r--   0 root         (0) root         (0)    14415 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/subnet.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/tag.py
+-rw-r--r--   0 root         (0) root         (0)     3821 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/volume.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc.py
+-rw-r--r--   0 root         (0) root         (0)     8498 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    10282 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.885219 idem-aws-1.7.5/idem_aws/tool/aws/ecr/
+-rw-r--r--   0 root         (0) root         (0)     4995 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ecr/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ecr/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.885219 idem-aws-1.7.5/idem_aws/tool/aws/efs/
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/efs/file_system_utils.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/efs/mount_target_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/efs/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.885219 idem-aws-1.7.5/idem_aws/tool/aws/eks/
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/addon.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4559 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/eks_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7710 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/nodegroup.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/eks/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.886219 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/
+-rw-r--r--   0 root         (0) root         (0)     9303 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    20325 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/elasticache_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elasticache/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.886219 idem-aws-1.7.5/idem_aws/tool/aws/elb/
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elb/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    19196 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elb/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elb/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.887219 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/
+-rw-r--r--   0 root         (0) root         (0)     7683 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10904 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/listener.py
+-rw-r--r--   0 root         (0) root         (0)    10107 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/load_balancer.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/tag.py
+-rw-r--r--   0 root         (0) root         (0)    10958 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/elbv2/target_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.887219 idem-aws-1.7.5/idem_aws/tool/aws/es/
+-rw-r--r--   0 root         (0) root         (0)     9741 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/es/elasticsearch_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/es/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.887219 idem-aws-1.7.5/idem_aws/tool/aws/events/
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/events/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5958 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/events/rule.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/events/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.888219 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/guardduty/detector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.889219 idem-aws-1.7.5/idem_aws/tool/aws/iam/
+-rw-r--r--   0 root         (0) root         (0)    12738 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/group.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/group_membership.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/password_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7466 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/policy.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/role_policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/service_linked_role.py
+-rw-r--r--   0 root         (0) root         (0)     3720 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/user.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/iam/user_ssh_key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.889219 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    21390 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/stream.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kinesis/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.889219 idem-aws-1.7.5/idem_aws/tool/aws/kms/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/alias.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/key.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/kms/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.890220 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/
+-rw-r--r--   0 root         (0) root         (0)     3194 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16057 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/init.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.890220 idem-aws-1.7.5/idem_aws/tool/aws/logs/
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/logs/subscription_filter_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.891219 idem-aws-1.7.5/idem_aws/tool/aws/neptune/
+-rw-r--r--   0 root         (0) root         (0)     8991 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     6385 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)    11654 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_instance.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_parameter_group.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_subnet_group.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/neptune/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/network_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.891219 idem-aws-1.7.5/idem_aws/tool/aws/organizations/
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/account.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/policy_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/organizations/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.892220 idem-aws-1.7.5/idem_aws/tool/aws/rds/
+-rw-r--r--   0 root         (0) root         (0)    12718 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/rds/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5582 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/rds/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.892220 idem-aws-1.7.5/idem_aws/tool/aws/route53/
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_association.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/resource_record_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/route53/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/s3/
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_acl.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     7403 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_logging.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_website.py
+-rw-r--r--   0 root         (0) root         (0)     9894 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/s3/s3_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/search_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/ses/
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/ses/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/sesv2/
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sesv2/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.893220 idem-aws-1.7.5/idem_aws/tool/aws/sns/
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sns/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7581 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sns/sns_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.894220 idem-aws-1.7.5/idem_aws/tool/aws/sqs/
+-rw-r--r--   0 root         (0) root         (0)     6482 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sqs/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/sqs/queue_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3760 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/state_utils.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/string_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/tag_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.894220 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/
+-rw-r--r--   0 root         (0) root         (0)     6843 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/ip_set_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/regex_pattern_set.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/wafv2/web_acl.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/aws/waiter_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.895220 idem-aws-1.7.5/idem_aws/tool/boto3/
+-rw-r--r--   0 root         (0) root         (0)     5000 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/client.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/custom_waiter.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/exception.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/region.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/resolve.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/boto3/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.895220 idem-aws-1.7.5/idem_aws/tool/heist/
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-05 18:38:25.000000 idem-aws-1.7.5/idem_aws/tool/heist/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:38:41.839216 idem-aws-1.7.5/idem_aws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11051 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22825 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 18:38:41.000000 idem-aws-1.7.5/idem_aws.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-05 18:38:25.000000 idem-aws-1.7.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:38:41.895220 idem-aws-1.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-05-05 18:38:25.000000 idem-aws-1.7.5/setup.py
```

### Comparing `idem-aws-1.7.4/LICENSE` & `idem-aws-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/PKG-INFO` & `idem-aws-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-aws
-Version: 1.7.4
+Version: 1.7.5
 Summary: AWS Cloud Provider for Idem
 Home-page: https://docs.idemproject.io/idem-aws/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-aws
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-aws/issues
```

### Comparing `idem-aws-1.7.4/README.rst` & `idem-aws-1.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/acct/aws/contracts/init.py` & `idem-aws-1.7.5/idem_aws/acct/aws/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/acct/aws/gsuite.py` & `idem-aws-1.7.5/idem_aws/acct/aws/gsuite.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/acct/aws/iam.py` & `idem-aws-1.7.5/idem_aws/acct/aws/iam.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/acct/aws/init.py` & `idem-aws-1.7.5/idem_aws/acct/aws/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/acct/metadata/aws.py` & `idem-aws-1.7.5/idem_aws/acct/metadata/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/function.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/init.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/param.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/param.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/plugin.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/possible_functions.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/possible_functions.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/resource.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/service.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/service.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/tag/plugin.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/tag/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/tag/template.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/tag/template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/template.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/utils/plugin.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/autogen/aws/utils/template.py` & `idem-aws-1.7.5/idem_aws/autogen/aws/utils/template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/conf.py` & `idem-aws-1.7.5/idem_aws/conf.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/esm/aws.py` & `idem-aws-1.7.5/idem_aws/esm/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/esm/contracts/aws.py` & `idem-aws-1.7.5/idem_aws/esm/contracts/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/acm/certificate_manager.py` & `idem-aws-1.7.5/idem_aws/exec/aws/acm/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/base_path_mapping.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/deployment.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/domain_name.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/integration.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/integration_response.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/method.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/method_response.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/resource.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/rest_api.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigateway/stage.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/api.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/authorizer.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/domain_name.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/integration.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/apigatewayv2/route.py` & `idem-aws-1.7.5/idem_aws/exec/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/application_autoscaling/scalable_target.py` & `idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/application_autoscaling/scaling_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/arn.py` & `idem-aws-1.7.5/idem_aws/exec/aws/arn.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/autoscaling/scaling_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/backup/backup_vault.py` & `idem-aws-1.7.5/idem_aws/exec/aws/backup/backup_vault.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/budgets/budget.py` & `idem-aws-1.7.5/idem_aws/exec/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/cloudformation/stack.py` & `idem-aws-1.7.5/idem_aws/exec/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/cloudfront/cache_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/cache_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/cloudfront/distribution.py` & `idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/distribution.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/cloudfront/origin_request_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/cloudfront/origin_request_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/cloudwatch/log_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/cloudwatchlogs/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/config/configuration_aggregator.py` & `idem-aws-1.7.5/idem_aws/exec/aws/config/configuration_aggregator.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py` & `idem-aws-1.7.5/idem_aws/exec/aws/costexplorer/cost_allocation_tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/data.py` & `idem-aws-1.7.5/idem_aws/exec/aws/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/docdb/db_cluster.py` & `idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/docdb/db_subnet_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/dynamodb/table.py` & `idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/dynamodb/tag.py` & `idem-aws-1.7.5/idem_aws/exec/aws/dynamodb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/ami.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/availability_zones.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/elastic_ip.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/flow_log.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/instance.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/instance_type.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/instance_type.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/internet_gateway.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/key_pair.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/launch_template.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/network_interface.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/placement_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/route.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/route_table.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/route_table_association.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/route_table_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/security_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/security_group_rule.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/snapshot.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/spot_instance_request.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/subnet.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/volume.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_endpoint.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_peering_connection.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_accepter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ec2/vpc_peering_connection_options.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ecr/image.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ecr/image.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ecr/lifecycle_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ecr/lifecycle_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ecr/repository.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ecr/repository_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ecr/repository_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/eks/cluster.py` & `idem-aws-1.7.5/idem_aws/exec/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/elasticache/replication_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/elasticache/replication_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/elb/elb_hosted_zone_id.py` & `idem-aws-1.7.5/idem_aws/exec/aws/elb/elb_hosted_zone_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/elb/load_balancer.py` & `idem-aws-1.7.5/idem_aws/exec/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/elbv2/listener.py` & `idem-aws-1.7.5/idem_aws/exec/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/elbv2/load_balancer.py` & `idem-aws-1.7.5/idem_aws/exec/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/elbv2/target_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/es/elasticsearch_domain.py` & `idem-aws-1.7.5/idem_aws/exec/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/events/rule.py` & `idem-aws-1.7.5/idem_aws/exec/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/guardduty/detector.py` & `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/guardduty/member.py` & `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/member.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/guardduty/organization_admin_account.py` & `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_admin_account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/guardduty/organization_configuration.py` & `idem-aws-1.7.5/idem_aws/exec/aws/guardduty/organization_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/access_key.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/access_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/group_membership.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/group_policy_attachment.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/group_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/instance_profile.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/instance_profile.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/open_id_connect_provider.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/open_id_connect_provider.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/password_policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/role.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/user.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/iam/user_policy_attachment.py` & `idem-aws-1.7.5/idem_aws/exec/aws/iam/user_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/kinesis/stream.py` & `idem-aws-1.7.5/idem_aws/exec/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/kms/key.py` & `idem-aws-1.7.5/idem_aws/exec/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-1.7.5/idem_aws/exec/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/neptune/db_instance.py` & `idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/neptune/db_parameter_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/organizations/account.py` & `idem-aws-1.7.5/idem_aws/exec/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/organizations/policy.py` & `idem-aws-1.7.5/idem_aws/exec/aws/organizations/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/rds/db_cluster.py` & `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/rds/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/rds/db_instance.py` & `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/rds/db_parameter_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/rds/db_subnet_group.py` & `idem-aws-1.7.5/idem_aws/exec/aws/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/rds/tag.py` & `idem-aws-1.7.5/idem_aws/exec/aws/rds/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/route53/hosted_zone.py` & `idem-aws-1.7.5/idem_aws/exec/aws/route53/hosted_zone.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket.py` & `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_acl.py` & `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_lifecycle.py` & `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_logging.py` & `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_replication.py` & `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/s3/bucket_website.py` & `idem-aws-1.7.5/idem_aws/exec/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ses/domain_identity.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ses/domain_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/ses/identity_notification_topic.py` & `idem-aws-1.7.5/idem_aws/exec/aws/ses/identity_notification_topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/sesv2/event_destination.py` & `idem-aws-1.7.5/idem_aws/exec/aws/sesv2/event_destination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/sns/subscription.py` & `idem-aws-1.7.5/idem_aws/exec/aws/sns/subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/sqs/queue.py` & `idem-aws-1.7.5/idem_aws/exec/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/sts/assume_role.py` & `idem-aws-1.7.5/idem_aws/exec/aws/sts/assume_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/sts/caller_identity.py` & `idem-aws-1.7.5/idem_aws/exec/aws/sts/caller_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/wafv2/ip_set.py` & `idem-aws-1.7.5/idem_aws/exec/aws/wafv2/ip_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/aws/wafv2/regex_pattern_set.py` & `idem-aws-1.7.5/idem_aws/exec/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/exec/boto3/init.py` & `idem-aws-1.7.5/idem_aws/exec/boto3/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/reconcile/pending/aws.py` & `idem-aws-1.7.5/idem_aws/reconcile/pending/aws.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/acm/certificate_manager.py` & `idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_manager.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/acm/certificate_validation.py` & `idem-aws-1.7.5/idem_aws/states/aws/acm/certificate_validation.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/base_path_mapping.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/base_path_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,24 +149,24 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    domain_name: str,
+    domain_name: str = None,
     base_path: str = None,
     resource_id: str = None,
 ):
     """
     Deletes the specified base path mapping.
 
     Args:
         name(str): The Idem name of the resource.
-        domain_name(str): the domain name of the BasePathMapping resource to delete.
+        domain_name(str, Optional): the domain name of the BasePathMapping resource to delete.
         base_path(str, Optional): The base path name of the BasePathMapping resource to delete.
                                     To specify an empty base path, set this parameter to '(none)' .
         resource_id(str, Optional): AWS Resource id. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
@@ -199,15 +199,24 @@
 
     if not before_ret["ret"]:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigateway.base_path_mapping", name=name
         )
         return result
 
-    elif ctx.get("test", False):
+    if not domain_name or not base_path:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.apigateway.base_path_mapping",
+            name=name,
+            args=["domain_name", "base_type"],
+        )
+        result["result"] = False
+        return result
+
+    if ctx.get("test", False):
         result["old_state"] = before_ret["ret"]
         result["comment"] = hub.tool.aws.comment_utils.would_delete_comment(
             resource_type="aws.apigateway.base_path_mapping", name=name
         )
         return result
 
     else:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/deployment.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,26 +205,26 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    rest_api_id: str,
+    rest_api_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Deletes a Deployment resource.
 
     Deleting a deployment will only succeed if there are no Stage resources associated with it.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        rest_api_id(str):
+        rest_api_id(str, Optional):
             The string identifier of the associated RestApi.
 
         resource_id(str, Optional):
             AWS API Gateway Deployment ID. Idem automatically considers this resource being absent if this field is not
             specified.
 
     Returns:
@@ -244,14 +244,23 @@
     if not resource_id:
         # if resource_id isn't specified, the resource is considered to be absent.
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigateway.deployment", name=name
         )
         return result
 
+    if not rest_api_id:
+        result["comment"] = result[
+            "comment"
+        ] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.apigateway.deployment", name=name, args=["rest_api_id"]
+        )
+        result["result"] = False
+        return result
+
     before_ret = await hub.exec.aws.apigateway.deployment.get(
         ctx,
         name=name,
         resource_id=resource_id,
         rest_api_id=rest_api_id,
     )
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/domain_name.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/integration.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/integration_response.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/method.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/method.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,30 +188,30 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    rest_api_id: str,
-    http_method: str,
-    parent_resource_id: str,
+    rest_api_id: str = None,
+    http_method: str = None,
+    parent_resource_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
 
     """Deletes an API Gateway Method resource
 
     Args:
-        name(str): An Idem name of the resource.
+        name(str, Optional): An Idem name of the resource.
 
-        parent_resource_id(str): AWS Parent Resource ID.
+        parent_resource_id(str, Optional): AWS Parent Resource ID.
 
-        rest_api_id(str): The string identifier of the associated RestApi.
+        rest_api_id(str, Optional): The string identifier of the associated RestApi.
 
-        http_method(str): The HTTP verb of the Method resource.
+        http_method(str, Optional): The HTTP verb of the Method resource.
 
         resource_id(str, Optional): The resource identifier for the Method resource. Idem automatically considers
             this resource being absent if this field is not specified.
 
     Returns:
         Dict[str, Any]
 
@@ -250,14 +250,25 @@
     if not before_ret["ret"]:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigateway.method", name=name
         )
 
     result["old_state"] = before_ret["ret"]
 
+    if not rest_api_id or not parent_resource_id or not http_method:
+        result["comment"] = result[
+            "comment"
+        ] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.apigateway.method",
+            name=name,
+            args=["rest_api_id", "parent_resource_id", "http_method"],
+        )
+        result["result"] = False
+        return result
+
     if ctx.get("test", False):
         result["comment"] = hub.tool.aws.comment_utils.would_delete_comment(
             resource_type="aws.apigateway.method", name=name
         )
         return result
 
     delete_ret = await hub.exec.boto3.client.apigateway.delete_method(
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/method_response.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/resource.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,22 +152,22 @@
         )
         result["new_state"] = resource_translated
 
     return result
 
 
 async def absent(
-    hub, ctx, name: str, rest_api_id: str, resource_id: str = None
+    hub, ctx, name: str, rest_api_id: str = None, resource_id: str = None
 ) -> Dict[str, Any]:
     """Deletes the specified resource.
 
     Args:
         name (str): The Idem name of the resource.
 
-        rest_api_id (str): AWS rest_api id of the associated RestApi.
+        rest_api_id (str, Optional): AWS rest_api id of the associated RestApi.
 
         resource_id (str, Optional): AWS Resource id. Defaults to None.
 
     Returns:
         dict[str, Any]
 
     Examples:
@@ -190,14 +190,21 @@
 
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigateway.resource", name=name
         )
         return result
 
+    if not rest_api_id:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.apigateway.resource", name=name, args=["rest_api_id"]
+        )
+        result["result"] = False
+        return result
+
     before_ret = await hub.exec.boto3.client.apigateway.get_resource(
         ctx, resourceId=resource_id, restApiId=rest_api_id
     )
 
     if not before_ret["result"]:
         if "NotFoundException" not in str(before_ret["comment"][0]):
             result["result"] = False
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/rest_api.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigateway/stage.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/api.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/authorizer.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/domain_name.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/integration.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,22 +318,22 @@
             return result
         result["new_state"] = after_ret["ret"]
 
     return result
 
 
 async def absent(
-    hub, ctx, name: str, api_id: str, resource_id: str = None
+    hub, ctx, name: str, api_id: str = None, resource_id: str = None
 ) -> Dict[str, Any]:
     """
     Deletes an API Gateway v2 integration resource.
 
     Args:
         name(str): An Idem name of the resource.
-        api_id(str): The API resource identifier in Amazon Web Services.
+        api_id(str, Optional): The API resource identifier in Amazon Web Services.
         resource_id(str, Optional): The Integration resource identifier in Amazon Web Services.
             Idem automatically considers this resource being absent if this field is not specified.
 
     Returns:
         Dict[str, Any]
 
     Examples:
@@ -351,14 +351,21 @@
 
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigatewayv2.integration", name=name
         )
         return result
 
+    if not api_id:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.apigateway2.integration", name=name, args=["api_id"]
+        )
+        result["result"] = False
+        return result
+
     before_ret = await hub.exec.aws.apigatewayv2.integration.get(
         ctx=ctx, name=name, resource_id=resource_id, api_id=api_id
     )
     if not before_ret["result"]:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigatewayv2.integration", name=name
         )
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/route.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,22 +234,22 @@
             api_id=api_id, raw_resource=after_ret.get("ret"), idem_resource_name=name
         )
 
     return result
 
 
 async def absent(
-    hub, ctx, name: str, api_id: str, resource_id: str = None
+    hub, ctx, name: str, api_id: str = None, resource_id: str = None
 ) -> Dict[str, Any]:
     """
     Deletes an API Gateway v2 route resource.
 
     Args:
         name(str): An Idem name of the resource.
-        api_id(str): The API resource identifier in Amazon Web Services.
+        api_id(str, Optional): The API resource identifier in Amazon Web Services.
         resource_id(str, Optional): The Route resource identifier in Amazon Web Services.
             Idem automatically considers this resource being absent if this field is not specified.
 
     Returns:
         Dict[str, Any]
 
     Examples:
@@ -267,14 +267,21 @@
 
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigatewayv2.route", name=name
         )
         return result
 
+    if not api_id:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.apigateway2.route", name=name, args=["api_id"]
+        )
+        result["result"] = False
+        return result
+
     before_ret = await hub.exec.boto3.client.apigatewayv2.get_route(
         ctx, ApiId=api_id, RouteId=resource_id
     )
     if not before_ret["result"]:
         if "NotFoundException" not in str(before_ret["comment"][0]):
             result["result"] = False
             result["comment"] = before_ret["comment"]
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/apigatewayv2/stage.py` & `idem-aws-1.7.5/idem_aws/states/aws/apigatewayv2/stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
             api_id=api_id, raw_resource=after_ret.get("ret")
         )
 
     return result
 
 
 async def absent(
-    hub, ctx, name: str, api_id: str, resource_id: str = None
+    hub, ctx, name: str, api_id: str = None, resource_id: str = None
 ) -> Dict[str, Any]:
     """
     Deletes an API Gateway v2 stage resource.
 
     Args:
         name(str): An Idem name of the resource.
         api_id(str): The API resource identifier in Amazon Web Services.
@@ -325,14 +325,21 @@
 
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.apigatewayv2.stage", name=name
         )
         return result
 
+    if not api_id:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.apigateway2.stage", name=name, args=["api_id"]
+        )
+        result["result"] = False
+        return result
+
     before_ret = await hub.exec.boto3.client.apigatewayv2.get_stage(
         ctx, ApiId=api_id, StageName=resource_id
     )
     if not before_ret["result"]:
         if "NotFoundException" not in str(before_ret["comment"][0]):
             result["result"] = False
             result["comment"] = before_ret["comment"]
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/application_autoscaling/scalable_target.py` & `idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scalable_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,33 +348,33 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    scaling_resource_id: str,
-    service_namespace: str,
-    scalable_dimension: str,
+    scaling_resource_id: str = None,
+    service_namespace: str = None,
+    scalable_dimension: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Deregisters an Application Auto Scaling scalable target when you have finished using it.
 
     To see which resources have been registered, use DescribeScalableTargets.
     Deregistering a scalable target deletes the scaling policies and the scheduled actions that are associated with it.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        service_namespace(str):
+        service_namespace(str, Optional):
             The namespace of the Amazon Web Services service that provides the resource. For a resource
             provided by your own application or service, use custom-resource instead.
 
-        scaling_resource_id(str):
+        scaling_resource_id(str, Optional):
             The identifier of the resource associated with the scalable target. This string consists of the
             resource type and unique identifier.
 
             * ECS service - The resource type is service and the unique identifier is the cluster name and service name.
               Example: service/default/sample-webapp.
             * Spot Fleet - The resource type is spot-fleet-request and the unique identifier is the Spot Fleet
               request ID. Example: spot-fleet-request/sfr-73fbd2ce-aa30-494c-8788-1cee4EXAMPLE.
@@ -410,15 +410,15 @@
               The resource type and unique identifier are specified using the cluster ARN. Example:
               arn:aws:kafka:us-east-1:123456789012:cluster/demo-cluster-1/6357e0b2-0e6a-4b86-a0b4-70df934c2e31-5.
             * Amazon ElastiCache replication group - The resource type is replication-group and the unique identifier
               is the replication group name. Example: replication-group/mycluster.
             * Neptune cluster - The resource type is cluster and the unique identifier is the cluster name. Example:
               cluster:mycluster.
 
-        scalable_dimension(str):
+        scalable_dimension(str, Optional):
             The scalable dimension associated with the scalable target. This string consists of the service
             namespace, resource type, and scaling property.
 
             * ecs:service:DesiredCount - The desired task count of an ECS service.
             * elasticmapreduce:instancegroup:InstanceCount - The instance count of an EMR Instance Group.
             * ec2:spot-fleet-request:TargetCapacity - The target capacity of a Spot Fleet.
             * appstream:fleet:DesiredCapacity - The desired capacity of an AppStream 2.0 fleet.
@@ -465,15 +465,27 @@
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.application_autoscaling.scalable_target", name=name
         )
         return result
+
     if resource_id:
+        if not service_namespace or not scaling_resource_id or not scalable_dimension:
+            result[
+                "comment"
+            ] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+                resource_type="aws.application_autoscaling.scalable_target",
+                name=name,
+                args=["service_namespace", "scaling_resource_id", "scalable_dimension"],
+            )
+            result["result"] = False
+            return result
+
         if not re.search(
             f"^({service_namespace})/({scaling_resource_id})/({scalable_dimension})$",
             resource_id,
         ):
             result["comment"] = (
                 f"Incorrect aws.application_autoscaling.scalable_target resource_id: {resource_id}. Expected id {service_namespace}/{scaling_resource_id}/{scalable_dimension}",
             )
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/application_autoscaling/scaling_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/application_autoscaling/scaling_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -575,38 +575,38 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    scaling_resource_id: str,
-    policy_name: str,
-    service_namespace: str,
-    scalable_dimension: str,
+    scaling_resource_id: str = None,
+    policy_name: str = None,
+    service_namespace: str = None,
+    scalable_dimension: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Deletes the specified scaling policy for an Application Auto Scaling scalable target.
 
     Deleting a step scaling policy deletes the underlying alarm action, but does not delete the CloudWatch alarm
     associated with the scaling policy, even if it no longer has an associated action. For more information, see
     Delete a step scaling policy and Delete a target tracking scaling policy in the Application Auto Scaling User Guide.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        policy_name(str):
+        policy_name(str, Optional):
             The name of the scaling policy.
 
-        service_namespace(str):
+        service_namespace(str, Optional):
             The namespace of the Amazon Web Services service that provides the resource.
             For a resource provided by your own application or service, use custom-resource instead.
 
-        scaling_resource_id(str):
+        scaling_resource_id(str, Optional):
             The identifier of the resource associated with the scalable target.
             This string consists of the resource type and unique identifier.
 
             * ECS service - The resource type is service and the unique identifier is the cluster name and service name.
               Example: service/default/sample-webapp.
             * Spot Fleet -
               The resource type is spot-fleet-request and the unique identifier is the Spot Fleet request ID.
@@ -643,15 +643,15 @@
               The resource type and unique identifier are specified using the cluster ARN.
               Example: arn:aws:kafka:us-east-1:123456789012:cluster/demo-cluster-1/6357e0b2-0e6a-4b86-a0b4-70df934c2e31-5.
             * Amazon ElastiCache replication group - The resource type is replication-group and the unique identifier
               is the replication group name. Example: replication-group/mycluster.
             * Neptune cluster -
               The resource type is cluster and the unique identifier is the cluster name. Example: cluster:mycluster.
 
-        scalable_dimension(str):
+        scalable_dimension(str, Optional):
             The scalable dimension. This string consists of the service namespace, resource type, and scaling property.
 
             * ecs:service:DesiredCount - The desired task count of an ECS service.
             * elasticmapreduce:instancegroup:InstanceCount - The instance count of an EMR Instance Group.
             * ec2:spot-fleet-request:TargetCapacity - The target capacity of a Spot Fleet.
             * appstream:fleet:DesiredCapacity - The desired capacity of an AppStream 2.0 fleet.
             * dynamodb:table:ReadCapacityUnits - The provisioned read capacity for a DynamoDB table.
@@ -709,14 +709,34 @@
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.application_autoscaling.scaling_policy", name=name
         )
         return result
+
+    if (
+        not service_namespace
+        or not scaling_resource_id
+        or not scalable_dimension
+        or not policy_name
+    ):
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.application_autoscaling.scaling_policy",
+            name=name,
+            args=[
+                "service_namespace",
+                "scaling_resource_id",
+                "scalable_dimension",
+                "policy_name",
+            ],
+        )
+        result["result"] = False
+        return result
+
     if not re.search(
         f"^({service_namespace})/({scaling_resource_id})/({scalable_dimension})/({policy_name})$",
         resource_id,
     ):
         result["comment"] = (
             f"Incorrect aws.application_autoscaling.scaling_policy resource_id: {resource_id}. Expected id {service_namespace}/{scaling_resource_id}/{scalable_dimension}/{policy_name}",
         )
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/autoscaling/auto_scaling_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/autoscaling/auto_scaling_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/autoscaling/launch_configuration.py` & `idem-aws-1.7.5/idem_aws/states/aws/autoscaling/launch_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/autoscaling/scaling_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/autoscaling/scaling_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -927,27 +927,27 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    auto_scaling_group_name: str,
+    auto_scaling_group_name: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Deletes the specified scaling policy.
 
     Deleting either a step scaling policy or a simple scaling policy deletes the underlying alarm action, but does not
     delete the alarm, even if it no longer has an associated action.
 
     Args:
         name(str):
             The name or Amazon Resource Name (ARN) of the scaling policy.
 
-        auto_scaling_group_name(str):
+        auto_scaling_group_name(str, Optional):
             The name of the Auto Scaling group.
 
         resource_id(str, Optional):
             policy name of an autoScalingGroup's policy.
 
     Request Syntax:
         .. code-block:: sls
@@ -972,14 +972,22 @@
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.autoscaling.scaling_policy", name=name
         )
         return result
+    if not auto_scaling_group_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.autoscaling.scaling_policy",
+            name=name,
+            args=["auto_scaling_group_name"],
+        )
+        result["result"] = False
+        return result
     before = await hub.exec.aws.autoscaling.scaling_policy.get(
         ctx=ctx,
         name=name,
         resource_id=resource_id,
         auto_scaling_group_name=auto_scaling_group_name,
     )
     if not before["result"]:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/backup/backup_vault.py` & `idem-aws-1.7.5/idem_aws/states/aws/backup/backup_vault.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/budgets/budget.py` & `idem-aws-1.7.5/idem_aws/states/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/budgets/budget_action.py` & `idem-aws-1.7.5/idem_aws/states/aws/budgets/budget_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,21 +316,21 @@
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
     return result
 
 
 async def absent(
-    hub, ctx, name: str, budget_name: str, resource_id: str = None
+    hub, ctx, name: str, budget_name: str = None, resource_id: str = None
 ) -> Dict[str, Any]:
     """Deletes an AWS Budget Action.
 
     Args:
         name(str): An Idem name of the AWS Budget Action.
-        budget_name(str): Budget Name
+        budget_name(str, Optional): Budget Name
         resource_id(str, Optional): Budget Action ID to identify the resource.
             Idem automatically considers this resource being absent if this field is not specified.
 
     Request Syntax:
         .. code-block:: sls
 
             [action-resource-id]:
@@ -358,14 +358,23 @@
 
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.budgets.budget_action", name=name
         )
         return result
 
+    if not account_id or not budget_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.budgets.budget_action",
+            name=name,
+            args=["account_id", "budget_name"],
+        )
+        result["result"] = False
+        return result
+
     before = await hub.exec.boto3.client.budgets.describe_budget_action(
         ctx, AccountId=account_id, BudgetName=budget_name, ActionId=resource_id
     )
 
     if not before:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.budgets.budget_action", name=name
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/caller_identity.py` & `idem-aws-1.7.5/idem_aws/states/aws/caller_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudformation/stack.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudfront/cache_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudfront/cache_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudfront/distribution.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudfront/distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str,
-    caller_reference: str,
     origins: make_dataclass(
         "Origins",
         [
             ("Quantity", int),
             (
                 "Items",
                 List[
@@ -265,16 +264,17 @@
                 field(default=None),
             ),
             ("MinTTL", int, field(default=None)),
             ("DefaultTTL", int, field(default=None)),
             ("MaxTTL", int, field(default=None)),
         ],
     ),
-    comment: str,
     enabled: bool,
+    comment: str = "",
+    caller_reference: str = "",
     logging: make_dataclass(
         "LoggingConfig",
         [("Enabled", bool), ("IncludeCookies", bool), ("Bucket", str), ("Prefix", str)],
     ) = None,
     viewer_certificate: make_dataclass(
         "ViewerCertificate",
         [
@@ -620,15 +620,15 @@
         make your updates. This helps to make sure that you include all the required fields. To view a summary, see
         Required Fields for Create Distribution and Update Distribution in the Amazon CloudFront Developer Guide.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        caller_reference (str):
+        caller_reference (str, Optional):
             A unique value (for example, a date-time stamp) that ensures that the request can't be replayed.
 
             If the value of CallerReference is new (regardless of the content of the DistributionConfig
             object), CloudFront creates a new distribution.
 
             If CallerReference is a value that you already sent in a previous request to create a distribution,
             CloudFront returns a DistributionAlreadyExists error.
@@ -1430,15 +1430,15 @@
               * ErrorCachingMinTTL (int, Optional):
                 The minimum amount of time, in seconds, that you want CloudFront to cache the HTTP status code specified
                 in ErrorCode. When this time period has elapsed, CloudFront queries your origin to see whether
                 the problem that caused the error has been resolved and the requested object is now available.
 
                 For more information, see Customizing Error Responses in the Amazon CloudFront Developer Guide.
 
-        comment(str):
+        comment(str, Optional):
                 An optional comment to describe the distribution. The comment cannot be longer than 128 characters.
 
         logging(dict, Optional):
             A complex type that controls whether access logs are written for the distribution.
 
             For more information about logging, see Access Logs in the Amazon CloudFront Developer Guide.
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudfront/origin_request_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudfront/origin_request_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudtrail/trail.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudwatch/log_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudwatch/metric_alarm.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudwatch/metric_alarm.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/cloudwatchlogs/resource_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/cloudwatchlogs/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/config/config_recorder.py` & `idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/config/config_recorder_status.py` & `idem-aws-1.7.5/idem_aws/states/aws/config/config_recorder_status.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/config/configuration_aggregator.py` & `idem-aws-1.7.5/idem_aws/states/aws/config/configuration_aggregator.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/config/delivery_channel.py` & `idem-aws-1.7.5/idem_aws/states/aws/config/delivery_channel.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/config/rule.py` & `idem-aws-1.7.5/idem_aws/states/aws/config/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/costexplorer/anomaly_monitor.py` & `idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,35 +308,42 @@
             result["new_state"] = copy.deepcopy(result["old_state"])
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes a cost anomaly monitor by the specified monitor ARN as resource_id.
 
     Args:
         name(str):
             The Idem name of the anomaly monitor.
-        resource_id(str):
+        resource_id(str, Optional):
             Monitor ARN to identify the resource.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             cost_monitor1234:
               aws.costexplorer.anomaly_monitor.absent:
                 - name: value
                 - resource_id: cost_monitor1234
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.costexplorer.anomaly_monitor", name=name
+        )
+        return result
+
     before = await hub.exec.boto3.client.ce.get_anomaly_monitors(
         ctx, MonitorArnList=[resource_id]
     )
 
     if before and before["ret"].get("AnomalyMonitors"):
         before = before["ret"]["AnomalyMonitors"][0]
     else:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/costexplorer/anomaly_subscription.py` & `idem-aws-1.7.5/idem_aws/states/aws/costexplorer/anomaly_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,21 +188,21 @@
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
 
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes a cost anomaly subscription.
 
     Args:
         name(str):
             An Idem name of the resource.
-        resource_id(str):
+        resource_id(str, Optional):
             Subscription ARN to identify the resource
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
@@ -210,14 +210,20 @@
             resource_is_absent:
               aws.costexplorer.anomaly_subscription.absent:
                 - name: value
                 - resource_id: value
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.costexplorer.anomaly_subscription", name=name
+        )
+        return result
+
     before = await hub.exec.boto3.client.ce.get_anomaly_subscriptions(
         ctx, SubscriptionArnList=[resource_id]
     )
     if not before["result"]:
         result["result"] = False
         result["comment"] = before["comment"]
         return result
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/costexplorer/cost_category.py` & `idem-aws-1.7.5/idem_aws/states/aws/costexplorer/cost_category.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/data.py` & `idem-aws-1.7.5/idem_aws/states/aws/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/docdb/db_cluster.py` & `idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/docdb/db_subnet_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/dynamodb/table.py` & `idem-aws-1.7.5/idem_aws/states/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/ami.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/dhcp_option.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/dhcp_option_association.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/dhcp_option_association.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,29 +146,29 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    vpc_id: str,
-    dhcp_id: str,
+    vpc_id: str = None,
+    dhcp_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """
     Deletes/disassociates association of DHCP options with VPC.
 
     Args:
         name(str):
             An Idem name to identify the dhcp option resource.
 
-        vpc_id (str):
+        vpc_id (str, Optional):
             AWS VPC ID that needs to be associated with dhcp options set.
 
-        dhcp_id (str):
+        dhcp_id (str, Optional):
             AWS DHCP Option Set ID.
 
         resource_id(str, Optional):
             Vpc ID and DHCP Options ID with a separator '-'. Format: [dhcp_id]-[vpc_id]
 
     Request Syntax:
         .. code-block:: sls
@@ -190,14 +190,29 @@
               aws.ec2.dhcp_option_association.absent:
                 - resource_id: dhcp-8dh27j-vpc-76db75b8
                 - vpc_id: vpc-76db75b8
                 - dhcp_id: dhcp-8dh27j
                 - name: my-dhcp-option
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+    if not resource_id:
+        result["comment"] = (
+            f"aws.ec2.dhcp_option_association '{name}' is already absent!",
+        )
+        return result
+
+    if not dhcp_id or not vpc_id:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.ec2.dhcp_option_association",
+            name=name,
+            args=["dhcp_id", "vpc_id"],
+        )
+        result["result"] = False
+        return result
+
     if resource_id:
         if not re.search(f"^({dhcp_id})-({vpc_id})$", resource_id):
             result[
                 "comment"
             ] = f"Incorrect aws.ec2.dhcp_option_association resource_id: {resource_id}. Expected id {dhcp_id}-{vpc_id}"
             result["result"] = False
             return result
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/elastic_ip.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/flow_log.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/instance.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/internet_gateway.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/key_pair.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/launch_template.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/nat_gateway.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/nat_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/network_interface.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/placement_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/placement_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,23 +184,23 @@
         result["new_state"] = copy.deepcopy(after["ret"])
     else:
         result["new_state"] = copy.deepcopy(result["old_state"])
 
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Delete an EC2 placement group if it exists.
 
     Deletes the specified placement group. You must terminate all instances in the placement group before you can
     delete the placement group. For more information, see Placement groups in the Amazon EC2 User Guide.
 
     Args:
         name(str): An Idem name of the resource and the GroupName of the placement group
-        resource_id(str):
+        resource_id(str, Optional):
             The GroupName of the placement group.
             Idem automatically considers this resource to be absent if this field is not specified.
 
     Request Syntax:
         .. code-block:: sls
 
             idem_placement_group_name:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/route.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/route_table.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/route_table_association.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/route_table_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/security_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/security_group_rule.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/snapshot.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,27 +164,27 @@
             result["new_state"] = copy.deepcopy(result["old_state"])
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deregisters the specified Snapshot
 
     Deletes the specified snapshot. When you make periodic snapshots of a volume, the snapshots are incremental, and
     only the blocks on the device that have changed since your last snapshot are saved in the new snapshot. When you
     delete a snapshot, only the data not needed for any other snapshot is removed. So regardless of which prior
     snapshots have been deleted, all active snapshots will have access to all the information needed to restore the
     volume. You cannot delete a snapshot of the root device of an EBS volume used by a registered AMI. You must
     first de-register the AMI before you can delete the snapshot. For more information, see Delete an Amazon EBS
     snapshot in the Amazon Elastic Compute Cloud User Guide.
 
     Args:
-        name (str): An Idem name of the snapshot.
+        name (str, Optional): An Idem name of the snapshot.
         resource_id(str): The snapshot ID.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/spot_instance_request.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/subnet.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/transit_gateway.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/volume.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,24 +237,24 @@
             result["new_state"] = copy.deepcopy(result["old_state"])
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deregisters the specified Volume
 
     Deletes the specified EBS volume. The volume must be in the available state (not attached to an instance). The
     volume can remain in the deleting state for several minutes. For more information, see Delete an Amazon EBS
     volume in the Amazon Elastic Compute Cloud User Guide.
 
     Args:
         name (str): An Idem name of the resource.
-        resource_id (str): Volume ID.
+        resource_id (str, Optional): Volume ID.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_endpoint.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_peering_connection.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_accepter.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,18 +172,18 @@
     It's not possible to delete vpc_peering_connection_accepter,
     You need to delete the vpc_peering_connection resource by calling vpc_peering_connection.absent,
     while providing the vpc_peering_connection id.
     If you want to modify the vpc_peering_connection_accepter resource,
     use the vpc_peering_connection_options.present.
 
     Args:
-        name:
+        name(str):
             An Idem name of the resource.
 
-        resource_id:
+        resource_id(str, Optional):
             The id of the vpc peering connection.
 
     Request Syntax:
         .. code-block:: sls
 
             [vpc-peering-connection-id]:
               aws.ec2.vpc_peering_connection_accepter.absent:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ec2/vpc_peering_connection_options.py` & `idem-aws-1.7.5/idem_aws/states/aws/ec2/vpc_peering_connection_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,18 +181,18 @@
     It's not possible to delete vpc_peering_connection_options,
     You need to delete the vpc_peering_connection resource by calling vpc_peering_connection.absent,
     while providing the vpc_peering_connection id.
     If you want to modify the vpc_peering_connection_options resource,
     use the vpc_peering_connection_options.present.
 
     Args:
-        name:
+        name(str):
             An Idem name of the resource.
 
-        resource_id:
+        resource_id(str, Optional):
             The id of the vpc peering connection.
 
     Request Syntax:
         .. code-block:: sls
 
             [vpc-peering-connection-id]:
               aws.ec2.vpc_peering_connection_options.absent:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ecr/lifecycle_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/ecr/lifecycle_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 ) -> Dict[str, Any]:
     """Deletes the lifecycle policy associated with the specified repository.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        repository_name(str):
+        repository_name(str, Optional):
             The name of the ECR repository in Amazon Web Services that contains the policy to delete.
 
         resource_id(str, Optional):
             The registry id and repository name with a separator '-'. Format: ``[registry_id]-[repository_name]``.
 
             .. warning::
               Idem automatically considers this resource being absent if this field is not specified.
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ecr/repository.py` & `idem-aws-1.7.5/idem_aws/states/aws/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ecr/repository_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/ecr/repository_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,24 +164,24 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    repository_name: str,
+    repository_name: str = None,
     resource_id: str = None,
     registry_id: str = None,
 ) -> Dict[str, Any]:
     """Deletes the policy associated with the specified AWS ECR repository.
 
     Args:
         name(str):
             An Idem name of the resource.
-        repository_name(str):
+        repository_name(str, Optional):
             The name of the ECR repository in Amazon Web Services that contains the policy to delete.
         resource_id(str, Optional):
             The registry id and repository name with a separator '-'. Format: ``[registry_id]-[repository_name]``.
 
             .. warning::
               Idem automatically considers this resource being absent if this field is not specified.
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/efs/file_system.py` & `idem-aws-1.7.5/idem_aws/states/aws/efs/file_system.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/efs/mount_target.py` & `idem-aws-1.7.5/idem_aws/states/aws/efs/mount_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         deletion by calling the DescribeMountTargets operation, which returns a list of mount target descriptions for
         the given file system.
 
     The operation also requires permissions for the following Amazon EC2 action on the mount target's network interface:
         * ``ec2:DeleteNetworkInterface``
 
     Args:
-        name(str, Optional):
+        name(str):
             An Idem name of the resource.
         resource_id(str, Optional):
             The ID of mount target.
         timeout(dict, Optional):
             Timeout configuration for deletion of AWS EFS mount target.
                 * delete (dict) -- Timeout configuration for deletion of an EFS mount target
                 * delay -- The amount of time in seconds to wait between attempts. Defaults to 15
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/eks/addon.py` & `idem-aws-1.7.5/idem_aws/states/aws/eks/addon.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    cluster_name: str,
+    cluster_name: str = None,
     resource_id: str = None,
     preserve: bool = False,
     timeout: Dict = None,
 ) -> Dict[str, Any]:
     """
     Delete an Amazon EKS add-on.
 
@@ -304,15 +304,15 @@
     cluster using the Kubernetes API.
 
     Args:
 
         name(str):
             An Idem name of the EKS addon resource.
 
-        cluster_name(str):
+        cluster_name(str, Optional):
             The name of the cluster to delete the add-on from.
 
         resource_id(str, Optional):
             AWS EKS addon name. Idem automatically considers this resource being absent if this field is not specified.
 
         preserve(bool, Optional):
             Specifying this option preserves the add-on software on your cluster but Amazon EKS stops managing any
@@ -350,14 +350,22 @@
 
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.eks.addon", name=name
         )
         return result
+
+    if not cluster_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.eks.addon", name=name, args=["cluster_name"]
+        )
+        result["result"] = False
+        return result
+
     before = await hub.exec.boto3.client.eks.describe_addon(
         ctx, clusterName=cluster_name, addonName=resource_id
     )
 
     if not before["ret"]:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.eks.addon", name=name
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/eks/cluster.py` & `idem-aws-1.7.5/idem_aws/states/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/eks/fargate_profile.py` & `idem-aws-1.7.5/idem_aws/states/aws/eks/fargate_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    cluster_name: str,
+    cluster_name: str = None,
     resource_id: str = None,
     timeout: Dict = None,
 ) -> Dict[str, Any]:
     """Deletes an Fargate profile.
 
     When you delete a Fargate profile, any pods running on Fargate that were created with the profile are deleted. If
     those pods match another Fargate profile, then they are scheduled on Fargate with that profile. If they no longer
@@ -271,15 +271,15 @@
     Fargate profile in a cluster can be in the DELETING status at a time. You must wait for a Fargate profile to finish
     deleting before you can delete any other profiles in that cluster.
 
     Args:
         name(str):
             An Idem name of the resource
 
-        cluster_name(str):
+        cluster_name(str, Optional):
             The name of the Amazon EKS cluster associated with the Fargate profile to delete.
 
         resource_id(str, Optional):
             AWS Fargate profile name. Idem considers name of fargate profile if
          this field is not specified.
 
         timeout(dict, Optional):
@@ -306,14 +306,28 @@
               aws.eks.fargate_profile.absent:
                 - resource_id: fargate01
                 - name: fargate01
                 - cluster_name: idem-cluster01
     """
 
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type=resource_type, name=name
+        )
+        return result
+
+    if not cluster_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type=resource_type, name=name, args=["cluster_name"]
+        )
+        result["result"] = False
+        return result
+
     before = await hub.exec.boto3.client.eks.describe_fargate_profile(
         ctx,
         clusterName=cluster_name,
         fargateProfileName=resource_id if resource_id else name,
     )
     if before and before["ret"]["fargateProfile"]:
         result[
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/eks/nodegroup.py` & `idem-aws-1.7.5/idem_aws/states/aws/eks/nodegroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,28 +508,28 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    cluster_name: str,
+    cluster_name: str = None,
     resource_id: str = None,
     timeout: Dict = None,
 ) -> Dict[str, Any]:
     """
     **Autogenerated function**
 
     Deletes an Amazon EKS node group for a cluster.
 
     Args:
         name(str):
             An Idem name of EKS Node group.
 
-        cluster_name(str):
+        cluster_name(str, None):
             The name of the cluster to create the node group in.
 
         resource_id(str, Optional):
             AWS EKS Node group name. Idem automatically considers this resource being absent
          if this field is not specified.
 
         timeout(dict, Optional):
@@ -562,14 +562,20 @@
 
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.eks.nodegroup", name=name
         )
         return result
+    if not cluster_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.eks.nodegroup", name=name, args=["cluster_name"]
+        )
+        result["result"] = False
+        return result
     before = await hub.exec.boto3.client.eks.describe_nodegroup(
         ctx, clusterName=cluster_name, nodegroupName=resource_id
     )
     if not before["ret"]:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.eks.nodegroup", name=name
         )
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/elasticache/cache_parameter_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/elasticache/cache_subnet_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/elasticache/cache_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/elasticache/replication_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/elasticache/replication_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/elb/load_balancer.py` & `idem-aws-1.7.5/idem_aws/states/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/elbv2/listener.py` & `idem-aws-1.7.5/idem_aws/states/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/elbv2/load_balancer.py` & `idem-aws-1.7.5/idem_aws/states/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/elbv2/target_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/es/elasticsearch_domain.py` & `idem-aws-1.7.5/idem_aws/states/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/events/rule.py` & `idem-aws-1.7.5/idem_aws/states/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/guardduty/detector.py` & `idem-aws-1.7.5/idem_aws/states/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/guardduty/member.py` & `idem-aws-1.7.5/idem_aws/states/aws/guardduty/member.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,28 +148,33 @@
         result["new_state"] = after["ret"]
     else:
         result["new_state"] = copy.deepcopy(result["old_state"])
     return result
 
 
 async def absent(
-    hub, ctx, name: str, detector_id: str, account_id: str, resource_id: str = None
+    hub,
+    ctx,
+    name: str,
+    detector_id: str = None,
+    account_id: str = None,
+    resource_id: str = None,
 ) -> Dict[str, Any]:
     r"""Delete member from AWS Guardduty.
 
     Deletes GuardDuty member account specified by the account ID.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        detector_id(str):
+        detector_id(str, Optional):
             AWS Guardduty Detector id
 
-        account_id(str):
+        account_id(str, Optional):
             AWS Guardduty member account id
 
         resource_id(str, Optional):
             An identifier refers to an existing resource. The format is <detector_id>:<account_id>
 
     Request Syntax:
       .. code-block:: sls
@@ -191,14 +196,30 @@
                 - name: test_delete_members
                 - detector_id: '68c25425ab84ea0dcae26311eddacd34'
                 - account_id: '106828723025'
                 - resource_id: '68c25425ab84ea0dcae26311eddacd34:106828723025'
     """
 
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.guardduty.member", name=name
+        )
+        return result
+
+    if not detector_id or not account_id:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.guardduty.member",
+            name=name,
+            args=["detector_id", "account_id"],
+        )
+        result["result"] = False
+        return result
+
     before = await hub.exec.aws.guardduty.member.get(
         ctx,
         detector_id=detector_id,
         account_id=account_id,
         resource_id=resource_id,
         name=name,
     )
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/guardduty/organization_admin_account.py` & `idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_admin_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,21 +111,21 @@
         result["new_state"] = account
     else:
         # already exists
         result["new_state"] = copy.deepcopy(result["old_state"])
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     r"""Disables an Amazon Web Services account within the Organization as the GuardDuty delegated administrator.
 
     Args:
         name(str):
             An Idem name of the resource.
-        resource_id(str):
+        resource_id(str, Optional):
             The Amazon Web Services Account ID for the organizations account to be disabled as a GuardDuty
             delegated administrator.
 
     Returns:
         Dict[str, Any]
 
     Examples:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/guardduty/organization_configuration.py` & `idem-aws-1.7.5/idem_aws/states/aws/guardduty/organization_configuration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/access_key.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/access_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,24 +135,24 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    user_name: str,
+    user_name: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """
     Ensure the specified access key does not exist.
     Both user_name and resource_id must be passed in.
 
     Args:
         name(str): An Idem name describing the resource.
-        user_name(str): AWS IAM user name that the key belongs to.
+        user_name(str, Optional): AWS IAM user name that the key belongs to.
         resource_id(str, Optional): AWS IAM access key ID.
     Returns:
         Dict[str, Any]
     Examples:
         .. code-block:: sls
 
             name_describing_key:
@@ -169,14 +169,21 @@
     }
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.iam.access_key", name=name
         )
         return result
 
+    if not user_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.iam.access_key", name=name, args=["user_name"]
+        )
+        result["result"] = False
+        return result
+
     # ------ look up key
     list_ret = await hub.exec.aws.iam.access_key.list(
         ctx, access_key_id=resource_id, user_name=user_name
     )
     result["comment"] = list_ret["comment"]
     if not list_ret["result"]:
         result["result"] = False
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/group.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes the specified IAM group.
 
     The group must not contain any users or have any attached policies.
 
     Args:
         name(str): An Idem name of the resource.
-        resource_id(str): Name of IAM group.
+        resource_id(str, Optional): Name of IAM group.
 
     Request Syntax:
         .. code-block:: sls
 
             [group_name]:
               aws.iam.group.absent:
                 - name: "string"
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/group_membership.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/group_membership.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,22 +127,22 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    users: List,
+    users: List = [],
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Removes users from the specified Group.
 
     Args:
         name(str): The name of the AWS IAM Group.
-        users(List): List of users to remove.
+        users(List, Optional): List of users to remove.
         resource_id(str): Name of IAM group.
 
     Request Syntax:
         .. code-block:: sls
 
             [group_name]:
               aws.iam.group.absent:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/group_policy_attachment.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/group_policy_attachment.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,28 +109,28 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    group: str,
-    policy_arn: str,
+    group: str = None,
+    policy_arn: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Removes the specified managed policy from the specified group.
 
     Args:
         name(str): An Idem name of the state.
 
-        group(str):
+        group(str, Optional):
             The name (friendly name, not ARN) of the IAM user to detach the policy from.
 
-        policy_arn(str):
-            The Amazon Resource Name (ARN) of the IAM policy you want to attach.
+        policy_arn(str, Optional):
+            The Amazon Resource Name (ARN) of the IAM policy you want to detach.
 
         resource_id(str, Optional): Policy ARN
 
     Request Syntax:
         .. code-block:: sls
 
             [iam-group-policy-name]:
@@ -156,14 +156,23 @@
 
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.iam.group_policy_attachment", name=name
         )
         return result
 
+    if not group or not policy_arn:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.iam.group_policy_attachment",
+            name=name,
+            args=["group", "policy_arn"],
+        )
+        result["result"] = False
+        return result
+
     before = await hub.exec.aws.iam.group_policy_attachment.get(
         ctx, name=name, group=group, resource_id=resource_id
     )
     if not before["result"]:
         result["comment"] = before["comment"]
         result["result"] = False
         return result
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/instance_profile.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/instance_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,21 @@
 
             instance-profile-test:
               aws.iam.instance_profile.absent:
                 - name: instance-profile-test
     """
 
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.iam.instance_profile", name=name
+        )
+        return result
+
     before = await hub.exec.aws.iam.instance_profile.get(
         ctx, name=name, resource_id=resource_id
     )
     if not before["result"]:
         result["comment"] = before["comment"]
         result["result"] = False
         return result
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/open_id_connect_provider.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/open_id_connect_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
     Deleting an IAM OIDC provider resource does not update any roles that reference the provider as a principal in their
     trust policies. Any attempt to assume a role that references a deleted provider fails.
 
     Args:
         name(str):
             The idem name for IAM OIDC provider.
 
-        resource_id(str):
+        resource_id(str, Optional):
             The Amazon Resource Name (ARN) of the IAM OpenID Connect provider resource object to delete.
 
     Request Syntax:
         [oidc-resource-id]:
           aws.iam.open_id_connect_provider.absent:
           - name: 'string'
           - resource_id: 'string'
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/password_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/role.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/role_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/role_policy_attachment.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/role_policy_attachment.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,29 +128,29 @@
         except hub.tool.boto3.exception.ClientError as e:
             result["comment"] = (f"{e.__class__.__name__}: {e}",)
             result["result"] = False
     return result
 
 
 async def absent(
-    hub, ctx, name: str, role_name: str, policy_arn: str
+    hub, ctx, name: str, role_name: str = None, policy_arn: str = None
 ) -> Dict[str, Any]:
     """Removes the specified managed policy from the specified role.
 
     Args:
         name(str):
             The name of the AWS IAM role policy.
 
-        role_name(str):
+        role_name(str, Optional):
             The name (friendly name, not ARN) of the role to attach a policy.
             This parameter allows (through its regex pattern) a string of characters consisting of upper
             and lowercase alphanumeric characters with no spaces.
             You can also include any of the following characters: _+=,.@-
 
-        policy_arn(str):
+        policy_arn(str, Optional):
             The Amazon Resource Name (ARN) of the IAM policy you want to attach.
 
     Request Syntax:
         .. code-block:: sls
 
             [rpa-resource-id]:
               aws.iam.role_policy_attachment.absent:
@@ -167,14 +167,21 @@
             resource_is_absent:
               aws.iam.role_policy_attachment.absent:
                 - name: value
                 - role_name: value
                 - policy_arn: value
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not role_name and not policy_arn:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.iam.role_policy_attachment", name=name
+        )
+        return result
+
     try:
         before_ret = (
             await hub.tool.aws.iam.role_policy_attachment.is_role_policy_attached(
                 ctx, role_name=role_name, policy_arn=policy_arn
             )
         )
     except hub.tool.boto3.exception.ClientError as e:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/service_linked_role.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/service_linked_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,22 @@
         name(str):
             AWS IAM service linked Role Name.
 
         resource_id(str, Optional):
             AWS IAM service linked Role Name. If not specified, Idem will use "name" parameter to identify the IAM service
             linked role on AWS.
 
+        timeout(Dict, Optional):
+            Timeout configuration for deletion of AWS service linked role.
+            * delete (dict):
+                Timeout configuration for deletion of a Nat Gateway
+                * delay: The amount of time in seconds to wait between attempts.
+                * max_attempts: Customized timeout configuration containing delay and max attempts.
+
+
     Request Syntax:
         .. code-block:: sls
 
             [service_linked_role-resource-id]:
               aws.iam.service_linked_role.absent:
                 - name: "string"
                 - resource_id: "string"
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/user.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
 
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes the specified IAM user.
 
     Unlike the Amazon Web Services Management Console, when you delete a user programmatically, you must delete the items
     attached to the user manually, or the deletion fails. For more information, see Deleting an IAM user.
     Before attempting to delete a user, remove the following items:
     Password (DeleteLoginProfile)   Access keys (DeleteAccessKey)   Signing certificate (DeleteSigningCertificate)
     SSH public key (DeleteSSHPublicKey)   Git credentials (DeleteServiceSpecificCredential)   Multi-factor
@@ -256,14 +256,21 @@
 
             user-1:
               aws.iam.user.absent:
                 - name: user-1
                 - resource_id: user-1
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.iam.user", name=name
+        )
+        return result
+
     resource = await hub.tool.boto3.resource.create(ctx, SERVICE, RESOURCE, resource_id)
     before = await hub.tool.boto3.resource.describe(resource)
 
     if not before:
         result["comment"] = (f"'{name}' already absent",)
     elif ctx.get("test", False):
         result[
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/user_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/user_policy_attachment.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/user_policy_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,22 @@
               aws.iam.user_policy_attachment.absent:
                 - name: test-policy-attachment
                 - user_name: serverless
                 - policy_arn: arn:aws:iam::aws:policy/AdministratorAccess
     """
 
     result = dict(comment=[], old_state=None, new_state=None, name=name, result=True)
+
+    if not user_name and not policy_arn:
+        result["comment"] += list(
+            hub.tool.aws.comment_utils.already_absent_comment(
+                resource_type="aws.iam.user_policy_attachment", name=name
+            )
+        )
+
     generated_resource_id = f"{user_name}/{policy_arn}"
     if resource_id and generated_resource_id != resource_id:
         result["comment"].append(
             f"resource_id mismatches. Use newly generated resource_id"
         )
     before_ret = await hub.exec.aws.iam.user_policy_attachment.get(
         ctx, name=name, user_name=user_name, policy_arn=policy_arn
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/iam/user_ssh_key.py` & `idem-aws-1.7.5/idem_aws/states/aws/iam/user_ssh_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,30 +175,30 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    user_name: str,
+    user_name: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Deletes the specified SSH public key.
 
     The SSH public key deleted by this operation is used only for authenticatingthe associated IAM user to an CodeCommit
     repository.
 
     Args:
         name(str):
             The name of the ssh public key to be deleted.
 
-        user_name(str):
+        user_name(str, Optional):
             The name (friendly name, not ARN) of the IAM user to delete the ssh public key from.
 
-        resource_id(str) :
+        resource_id(str, Optional) :
             The ID of the ssh public key to be deleted.
 
     Request Syntax:
         .. code-block:: sls
 
             [iam-user-ssh-key-id]:
               aws.iam.user_ssh_key.absent:
@@ -216,14 +216,30 @@
               aws.iam.user_ssh_key.absent:
                 - user_name:  my-iam-user-1
                 - name: APKASYLXZO1EQCR0ZAL7
                 - resource_id: APKASYLXZO1EQCR0ZAL7
     """
 
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id and not user_name:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.iam.user_ssh_key", name=name
+        )
+        return result
+
+    if not resource_id or not user_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.iam.user_ssh_key",
+            name=name,
+            args=["resource_id", "user_name"],
+        )
+        result["result"] = False
+        return result
+
     before_ret = await hub.tool.aws.iam.user_ssh_key.get_ssh_key_if_attached_to_user(
         ctx, user_name=user_name, ssh_public_key_id=resource_id
     )
     if not before_ret["result"]:
         result["result"] = False
         result["comment"] = before_ret["comment"]
         return result
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/kinesis/stream.py` & `idem-aws-1.7.5/idem_aws/states/aws/kinesis/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
     You can use the DescribeStreamSummary operation to check the state of the stream, which is returned in StreamStatus.
     DeleteStream has a limit of five transactions per second and per account.
 
     Args:
         name(str):
             An Idem name of the resource.
 
-        resource_id(str):
+        resource_id(str, Optional):
             An identifier of the resource in the provider.
 
         enforce_consumer_deletion(bool, Optional):
             If this parameter is unset (null) or if you set it to false, and the stream has registered consumers, the
             call to DeleteStream fails with a ResourceInUseException. Defaults to None.
 
         timeout(dict, Optional):
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/kms/alias.py` & `idem-aws-1.7.5/idem_aws/states/aws/kms/alias.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/kms/key.py` & `idem-aws-1.7.5/idem_aws/states/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function.py` & `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function_permission.py` & `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,23 +209,23 @@
         resource_type="aws.lambda_aws.function_permission", name=name
     )
 
     return result
 
 
 async def absent(
-    hub, ctx, name: str, function_name: str, resource_id: str = None
+    hub, ctx, name: str, function_name: str = None, resource_id: str = None
 ) -> Dict[str, Any]:
     """Remove specified permission from the lambda function.
 
     Args:
         name(str):
             Name/Id of the statement/permission
 
-        function_name(str):
+        function_name(str, Optional):
             The name of the Lambda function, version, or alias.
                 Name formats
                     * Function name - my-function (name-only), my-function:v1 (with alias).
                     * Function ARN - ``arn:aws:lambda:us-west-2:123456789012:function:my-function`` .
                     * Partial ARN - ``123456789012:function:my-function`` .
 
         resource_id(str, Optional):
@@ -247,14 +247,26 @@
             test_idem_lambda_function_statement:
               aws.lambda_aws.function_permission.absent:
               - name: test-001
 
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
+    if not resource_id:
+        resource_id = name
+
+    if not function_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.lambda_aws.function_permission",
+            name=name,
+            args=["function_name"],
+        )
+        result["result"] = False
+        return result
+
     ret = await hub.exec.boto3.client["lambda"].get_function(
         ctx, FunctionName=function_name
     )
     if not ret["result"]:
         result["comment"] = ret["comment"]
         result["result"] = False
         return result
@@ -292,31 +304,30 @@
                 function_name=function_name,
                 revision_id=get_policy["ret"]["RevisionId"],
             )
             break
 
     if ctx.get("test", False):
         result["comment"] = hub.tool.aws.comment_utils.would_delete_comment(
-            resource_type="aws.lambda_aws.function_permission",
-            name=resource_id if resource_id else name,
+            resource_type="aws.lambda_aws.function_permission", name=resource_id
         )
         return result
 
     remove_permission = await hub.exec.boto3.client["lambda"].remove_permission(
         ctx,
         FunctionName=function_name,
-        StatementId=resource_id if resource_id else name,
+        StatementId=resource_id,
     )
     if not remove_permission["result"]:
         result["comment"] = remove_permission["comment"]
         result["result"] = False
 
     result["comment"] = hub.tool.aws.comment_utils.delete_comment(
         resource_type="aws.lambda_aws.function_permission",
-        name=resource_id if resource_id else name,
+        name=resource_id,
     )
 
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     """Returns permissions associated with each lambda function.
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-1.7.5/idem_aws/states/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/logs/subscription_filter.py` & `idem-aws-1.7.5/idem_aws/states/aws/logs/subscription_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,24 +168,24 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    log_group_name: str,
+    log_group_name: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """
 
     Deletes the specified subscription filter.
 
     Args:
         name(str): An Idem name of the resource.
-        log_group_name(str): The name of the log group.
+        log_group_name(str, Optional): The name of the log group.
         resource_id(str, Optional): AWS logs Subscription filter name. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
 
@@ -201,14 +201,22 @@
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     before = None
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.logs.subscription_filter", name=name
         )
         return result
+    if not log_group_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.logs.subscription_filter",
+            name=name,
+            args=["log_group_name"],
+        )
+        result["result"] = False
+        return result
     ret = await hub.exec.boto3.client.logs.describe_subscription_filters(
         ctx, logGroupName=log_group_name, filterNamePrefix=resource_id
     )
     if not ret["result"]:
         result["result"] = False
         result["comment"] = ret["comment"]
         return result
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/neptune/db_cluster.py` & `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/neptune/db_instance.py` & `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/neptune/db_parameter_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/neptune/db_subnet_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/neptune/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/organizations/account.py` & `idem-aws-1.7.5/idem_aws/states/aws/organizations/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,27 +319,27 @@
 
     else:
         result["new_state"] = copy.deepcopy(result["old_state"])
 
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Removes the specified account from the organization.
 
     The removed account becomes a standalone account that isn't a member of any organization.
     It's no longer subject to any policies and is responsible for its own bill payments.
     The organization's management account is no longer charged for any expenses accrued by
     the member account after it's removed from the organization.
     This operation can be called only from the organization's management account.
 
     Args:
         name(str):
             The name of the member account.
-        resource_id(str):
+        resource_id(str, Optional):
             The ID of the member account in Amazon Web Services.
 
     Request syntax:
       .. code-block:: sls
 
         [idem_test_aws_organizations_account]:
           aws.organizations.account.absent:
@@ -355,14 +355,21 @@
             idem_test_aws_organizations_account:
               aws.organizations.account.absent:
                 - name: 'idem_test_account'
                 - resource_id: '123456789012'
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.organizations.account",
+            name=name,
+        )
+        return result
+
     before = await hub.exec.aws.organizations.account.get(
         ctx, resource_id=resource_id, name=name
     )
 
     if not before["result"]:
         result["result"] = before["result"]
         result["comment"] = before["comment"]
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/organizations/organization.py` & `idem-aws-1.7.5/idem_aws/states/aws/organizations/organization.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/organizations/organization_unit.py` & `idem-aws-1.7.5/idem_aws/states/aws/organizations/organization_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,24 +245,24 @@
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
 
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes an organizational unit (OU) from a root or another OU.
 
     You must first remove all accounts and child OUs from the OU that you want to delete.
     This operation can be called only from the organization's management account.
 
     Args:
         name(str):
             An Idem name of the resource.
-        resource_id(str):
+        resource_id(str, Optional):
             The ID of the organization unit in Amazon Web Services.
 
     Request syntax:
       .. code-block:: sls
 
         [idem_test_aws_organizations_organization_unit]:
           aws.organizations.organization_unit.absent:
@@ -278,14 +278,21 @@
             idem_test_aws_organizations_organization_unit:
               aws.organizations.organization_unit.absent:
                 - name: 'idem_test_organization_unit'
                 - resource_id: 'ou-rootid-ouid'
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.organizations.organization_unit",
+            name=name,
+        )
+        return result
+
     before = await hub.exec.boto3.client.organizations.describe_organizational_unit(
         ctx, OrganizationalUnitId=resource_id
     )
 
     if not before:
         result["comment"] = result["comment"] + (
             f"aws.organizations.organization_unit '{name}' already absent",
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/organizations/policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/organizations/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
     """Deletes the specified policy from your organization.
 
     Before you perform this operation, you must first detach the policy from all organizational units (OUs), roots,
     and accounts. This operation can be called only from the organization's management account.
 
     Args:
         name(str): The name of the policy.
-        resource_id(str): The ID of the policy in Amazon Web Services.
+        resource_id(str, Optional): The ID of the policy in Amazon Web Services.
 
     Request syntax:
       .. code-block:: sls
 
           [idem_test_aws_organizations_policy]:
             aws.organizations.policy.absent:
               - name: 'string'
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/organizations/policy_attachment.py` & `idem-aws-1.7.5/idem_aws/states/aws/organizations/policy_attachment.py`

 * *Files 7% similar despite different names*

```diff
@@ -118,15 +118,17 @@
             )
         except hub.tool.boto3.exception.ClientError as e:
             result["comment"] = result["comment"] + (f"{e.__class__.__name__}: {e}",)
             result["result"] = False
     return result
 
 
-async def absent(hub, ctx, name: str, policy_id: str, target_id: str) -> Dict[str, Any]:
+async def absent(
+    hub, ctx, name: str, policy_id: str = None, target_id: str = None
+) -> Dict[str, Any]:
     """Detaches a policy from a target root, organizational unit (OU), or account.
 
     .. warning::
         If the policy being detached is a service control policy (SCP), the changes to permissions for
         Identity and Access Management (IAM) users and roles in affected accounts are immediate.
 
     Every root, OU, and account must have at least one SCP attached. If you want to replace the default
@@ -135,17 +137,17 @@
     ``allow list``. If you instead attach a second SCP and leave the ``FullAWSAccess`` SCP still attached,
     and specify ``"Effect": "Deny"`` in the second SCP to override the ``"Effect": "Allow"`` in the
     ``FullAWSAccess`` policy (or any other attached SCP), you're using the authorization strategy of a ``deny list``.
 
     Args:
         name(str):
             An Idem name of the resource.
-        policy_id(str):
+        policy_id(str, Optional):
             The unique identifier (ID) of the policy you want to detach.
-        target_id(str):
+        target_id(str, Optional):
             The unique identifier (ID) of the root, OU, or account that you want to detach the policy from.
 
     Request syntax:
       .. code-block:: sls
 
         [idem_test_aws_organizations_policy_attachment]:
           aws.organizations.policy_attachment.absent:
@@ -163,14 +165,29 @@
               aws.organizations.policy_attachment.absent:
                 - name: 'idem_test_policy_attachment'
                 - policy_id: 'p-123456789012'
                 - target_id: 'ou-root-id'
     """
     result = dict(comment=(), name=name, result=True, old_state=None, new_state=None)
 
+    if not policy_id and not target_id:
+        result["comment"] = (
+            f"aws.organizations.policy_attachment. '{name}' already absent",
+        )
+        return result
+
+    if not policy_id or not target_id:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.organizations.policy_attachment",
+            name=name,
+            args=["policy_id", "target_id"],
+        )
+        result["result"] = False
+        return result
+
     try:
         before_ret = await hub.tool.aws.organizations.policy_attachment.is_target_policy_attached(
             ctx, policy_id=policy_id, target_id=target_id
         )
     except hub.tool.boto3.exception.ClientError as e:
         result["comment"] = (f"{e.__class__.__name__}: {e}",)
         result["result"] = False
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/rds/db_cluster.py` & `idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/rds/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/rds/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/rds/db_instance.py` & `idem-aws-1.7.5/idem_aws/states/aws/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/rds/db_parameter_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/rds/db_parameter_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,25 +264,25 @@
             result["new_state"] = copy.deepcopy(result["old_state"])
     except Exception as e:
         result["comment"] += (str(e),)
         result["result"] = False
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes a specified DB parameter group.
 
     The DB parameter group to be deleted can't be associated with any DB
     instances.
 
     Args:
         resource_id(str):
             An identifier of the resource in the provider.
 
-        name(str):
+        name(str, Optional):
             The name of the DB parameter group.
 
             Constraints:
 
               * Must be the name of an existing DB parameter group.
               * You can't delete a default DB parameter group.
               * Can't be associated with any DB instances.
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/rds/db_subnet_group.py` & `idem-aws-1.7.5/idem_aws/states/aws/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/route53/hosted_zone.py` & `idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/route53/hosted_zone_association.py` & `idem-aws-1.7.5/idem_aws/states/aws/route53/hosted_zone_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/route53/resource_record.py` & `idem-aws-1.7.5/idem_aws/states/aws/route53/resource_record.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_acl.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_encryption.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_lifecycle.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_logging.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_notification.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_notification.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,25 +187,25 @@
     return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    bucket: str,
+    bucket: str = None,
     resource_id: str = None,
     expected_bucket_owner: str = None,
 ) -> Dict[str, Any]:
     """Deletes the policy of specified s3 bucket.
 
     Args:
         name(str):
             The name of the bucket policy.
 
-        bucket(str):
+        bucket(str, Optional):
             The name of the S3 bucket
 
         resource_id(str, Optional):
             S3 Bucket policy ID. Idem automatically considers this resource being absent if this field is not specified.
 
         expected_bucket_owner(str, Optional):
             The account ID of the expected bucket owner. If the bucket is owned by a different account, the request
@@ -232,14 +232,21 @@
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             resource_type="aws.s3.bucket_policy", name=name
         )
         return result
 
+    if not bucket:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.s3.bucket_policy", name=name, args=["bucket"]
+        )
+        result["result"] = False
+        return result
+
     if resource_id.split("-policy")[0] != bucket:
         result["comment"] = (f"Incorrect aws.s3.bucket name: '{bucket}'",)
         result["result"] = False
         return result
 
     # Check if bucket exists.
     ret = await hub.exec.boto3.client.s3.head_bucket(ctx, Bucket=bucket)
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_replication.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_versioning.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/bucket_website.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/bucket_website.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,18 @@
         result["old_state"] = copy.deepcopy(before["ret"])
         result["new_state"] = copy.deepcopy(result["old_state"])
 
         result["comment"] += list(
             hub.tool.aws.comment_utils.already_exists_comment("aws.s3.bucket", name)
         )
         if not data.recursive_diff(
-            website_configuration, result["old_state"]["website_configuration"]
+            website_configuration,
+            result["old_state"]["website_configuration"],
+            ignore_missing_keys=True,
+            ignore_order=True,
         ):
             # no updates to make. return from here
             return result
 
         if ctx.get("test", False):
             result["new_state"]["website_configuration"] = website_configuration
             result["comment"] += list(
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/s3/public_access_block.py` & `idem-aws-1.7.5/idem_aws/states/aws/s3/public_access_block.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ses/domain_identity.py` & `idem-aws-1.7.5/idem_aws/states/aws/ses/domain_identity.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/ses/identity_notification_topic.py` & `idem-aws-1.7.5/idem_aws/states/aws/ses/identity_notification_topic.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/sesv2/event_destination.py` & `idem-aws-1.7.5/idem_aws/states/aws/sesv2/event_destination.py`

 * *Files 6% similar despite different names*

```diff
@@ -231,30 +231,30 @@
         except Exception as e:
             result["comment"] = result["comment"] + (f"{e.__class__.__name__}: {e}",)
             result["result"] = False
     return result
 
 
 async def absent(
-    hub, ctx, name: str, configuration_set_name: str, resource_id: str = None
+    hub, ctx, name: str, configuration_set_name: str = None, resource_id: str = None
 ) -> Dict[str, Any]:
     """Delete an event destination.
 
     Events include message sends, deliveries, opens, clicks, bounces, and complaints.
     Event destinations are places that you can send information about these events to. For example, you can send
     event data to Amazon SNS to receive notifications when you receive bounces or complaints, or you can use Amazon
     Kinesis Data Firehose to stream data to Amazon S3 for long-term storage.
 
     Args:
-        resource_id(str, Optional):
-            An identifier of the resource in the provider.
         name(str):
             The name of the event destination to delete.
-        configuration_set_name(str):
+        configuration_set_name(str, Optional):
             The name of the configuration set that contains the event destination to delete.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider.
 
     Returns:
         .. code-block:: bash
 
             {"result": True|False, "comment": ("A tuple",), "ret": None|Dict}
 
 
@@ -263,58 +263,67 @@
 
             resource_is_absent:
               aws.sesv2.event_destination.absent:
                 - name: value
                 - resource_id: value
                 - configuration_set_name: value
     """
-    result, exists = (
-        dict(comment=(), old_state=None, new_state=None, name=name, result=True),
-        False,
-    )
+    result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.sesv2.event_destination", name=name
+        )
+        return result
+
+    if not configuration_set_name:
+        result["comment"] = hub.tool.aws.comment_utils.missing_args_for_absent_comment(
+            resource_type="aws.sesv2.event_destination",
+            name=name,
+            args=["configuration_set_name"],
+        )
+        result["result"] = False
+        return result
 
     before = await hub.exec.aws.sesv2.event_destination.get(
         ctx=ctx,
-        resource_id=name,
+        resource_id=resource_id,
         configuration_set_name=configuration_set_name,
     )
 
     if not before["result"]:
         result["comment"] = before["comment"]
         result["result"] = False
         return result
 
-    if before.get("ret"):
-        exists = True
-        result["old_state"] = before["ret"].copy()
-
-    if not exists:
-        result["comment"] = getattr(
-            hub.tool.aws.comment_utils, "already_absent_comment"
-        )(resource_type="aws.sesv2.event_destination", name=name)
-    elif ctx.get("test", False):
-        result["comment"] = getattr(hub.tool.aws.comment_utils, "would_delete_comment")(
+    if not before.get("ret"):
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.sesv2.event_destination", name=name
+        )
+        return result
+
+    if ctx.get("test", False):
+        result["comment"] = hub.tool.aws.comment_utils.would_delete_comment(
             resource_type="aws.sesv2.event_destination", name=name
         )
         return result
     else:
         try:
             ret = await hub.exec.boto3.client.sesv2.delete_configuration_set_event_destination(
                 ctx,
                 **{
                     "ConfigurationSetName": configuration_set_name,
-                    "EventDestinationName": name,
+                    "EventDestinationName": resource_id,
                 },
             )
-            result["result"] = ret["result"]
             if not result["result"]:
                 result["comment"] = ret["comment"]
                 result["result"] = False
                 return result
-            result["comment"] = getattr(hub.tool.aws.comment_utils, "delete_comment")(
+            result["comment"] = hub.tool.aws.comment_utils.delete_comment(
                 resource_type="aws.sesv2.event_destination", name=name
             )
         except Exception as e:
             result["result"] = False
             result["comment"] = result["comment"] + (f"{e.__class__.__name__}: {e}",)
 
     return result
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/sns/subscription.py` & `idem-aws-1.7.5/idem_aws/states/aws/sns/subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,24 +178,24 @@
             result["new_state"] = copy.deepcopy(result["old_state"])
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes the specified subscription.
 
     This action is idempotent, so deleting a topic that does not exist does not result in an error.
 
     Args:
         name(str):
             The name of the state.
 
-        resource_id(str):
+        resource_id(str, Optional):
             The AWS resource identifier i.e. resource arn
 
     Request Syntax:
         .. code-block:: yaml
 
             [subscription-name]:
               aws.sns.subscription.absent:
@@ -208,14 +208,21 @@
         .. code-block:: yaml
 
             test-subscription:
               aws.sns.subscription.absent:
               - resource_id: arn:aws:sns:eu-west-3:537227425989:test-topic:9c0fd640-7fc6-4888-bc08-f0a497a6237f
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.sns.subscription", name=name
+        )
+        return result
+
     before = None
 
     # There is a delay with describe() call, to check if the resource is in list_subscriptions() before describe()
     ret = await hub.exec.boto3.client.sns.list_subscriptions(ctx)
     if not ret["result"]:
         result["result"] = False
         result["comment"] = ret["comment"]
@@ -225,35 +232,41 @@
             resource = await hub.tool.boto3.resource.create(
                 ctx, "sns", "Subscription", arn=resource_id
             )
             before = await hub.tool.boto3.resource.describe(resource)
             break
 
     if not before:
-        result["comment"] = (f"aws.sns.subscription '{name}' already absent",)
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.sns.subscription", name=name
+        )
 
     else:
         result[
             "old_state"
         ] = hub.tool.aws.sns.conversion_utils.convert_raw_subscription_to_present(
             raw_resource=before, idem_resource_name=name
         )
         if ctx.get("test", False):
-            result["comment"] = (f"Would delete aws.sns.subscription '{name}'",)
+            result["comment"] = hub.tool.aws.comment_utils.would_delete_comment(
+                resource_type="aws.sns.subscription", name=name
+            )
             return result
         try:
             ret = await hub.exec.boto3.client.sns.unsubscribe(
                 ctx, SubscriptionArn=resource_id
             )
             result["result"] = ret["result"]
             if not result["result"]:
                 result["comment"] = ret["comment"]
                 result["result"] = False
                 return result
-            result["comment"] = (f"Deleted aws.sns.subscription '{name}'",)
+            result["comment"] = hub.tool.aws.comment_utils.delete_comment(
+                resource_type="aws.sns.subscription", name=name
+            )
         except hub.tool.boto3.exception.ClientError as e:
             result["comment"] = result["comment"] + (f"{e.__class__.__name__}: {e}",)
 
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/sns/topic.py` & `idem-aws-1.7.5/idem_aws/states/aws/sns/topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,25 +214,25 @@
             result["new_state"] = copy.deepcopy(result["old_state"])
     except Exception as e:
         result["comment"] = result["comment"] + (str(e),)
         result["result"] = False
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes a topic and all its subscriptions.
 
     Deleting a topic might prevent some messages previously sent to the topic from being delivered to subscribers. This
     action is idempotent, so deleting a topic that does not exist does not result in an error.
 
     Args:
         name(str):
             The name of the state.
 
-        resource_id(str):
+        resource_id(str, Optional):
             The AWS resource identifier, here it is resource arn
 
     Request Syntax:
         .. code-block:: yaml
 
             [topic-name]:
               aws.sns.topic.absent:
@@ -245,14 +245,19 @@
         .. code-block:: yaml
 
             test-topic:
               aws.sns.topic.absent:
                 - resource_id: arn:aws:sns:eu-west-3:537227425989:test-topic
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.sns.topic", name=name
+        )
+        return result
     resource = await hub.tool.boto3.resource.create(ctx, "sns", "Topic", resource_id)
     before = await hub.tool.boto3.resource.describe(resource)
 
     if not before:
         result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
             "aws.sns.topic", name
         )
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/sns/topic_policy.py` & `idem-aws-1.7.5/idem_aws/states/aws/sns/topic_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,38 +126,43 @@
             raw_resource=after, idem_resource_name=name
         )
     else:
         result["new_state"] = copy.deepcopy(result["old_state"])
     return result
 
 
-async def absent(hub, ctx, name: str, resource_id: str) -> Dict[str, Any]:
+async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
     """Deletes the current topic policy and replace with the default value.
 
     This action is idempotent, so deleting a topic's policy that does not exist does not result in an error.
 
     Args:
         name(str):
             The idem name of the topic_policy.
 
-        resource_id(str):
+        resource_id(str, Optional):
             Topic arn and 'policy' keyword separated with '-'
 
     Returns:
         dict[str, Any]
 
     Examples:
         .. code-block:: yaml
 
             test-topic-policy:
               aws.sns.topic_policy.absent:
               - name: test-topic-policy
               - resource_id: arn:aws:sns:eu-west-3:537227425989:test-topic-policy
     """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
+    if not resource_id:
+        result["comment"] = hub.tool.aws.comment_utils.already_absent_comment(
+            resource_type="aws.sns.topic_policy", name=name
+        )
+        return result
     topic_arn = resource_id.split("-policy")[0]
     before = await hub.exec.boto3.client.sns.get_topic_attributes(
         ctx, TopicArn=topic_arn
     )
 
     if not before:
         result["comment"] = (f"aws.sns.topic with '{topic_arn}' ARN does not exist",)
```

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/sqs/queue.py` & `idem-aws-1.7.5/idem_aws/states/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/wafv2/associate_web_acl.py` & `idem-aws-1.7.5/idem_aws/states/aws/wafv2/associate_web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/wafv2/ip_set.py` & `idem-aws-1.7.5/idem_aws/states/aws/wafv2/ip_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/wafv2/regex_pattern_set.py` & `idem-aws-1.7.5/idem_aws/states/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/states/aws/wafv2/web_acl.py` & `idem-aws-1.7.5/idem_aws/states/aws/wafv2/web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/acct/assume_role.py` & `idem-aws-1.7.5/idem_aws/tool/aws/acct/assume_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/acct/init.py` & `idem-aws-1.7.5/idem_aws/tool/aws/acct/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/acct/key_name.py` & `idem-aws-1.7.5/idem_aws/tool/aws/acct/key_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/acm/certificate_validation_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/acm/certificate_validation_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/acm/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/acm/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/acm/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/acm/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/base_path_mapping.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/base_path_mapping.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/deployment.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/deployment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/domain_name.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/integration.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/integration_response.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/integration_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/method.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/method_response.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/method_response.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/resource.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/rest_api.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/rest_api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/stage.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigateway/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigateway/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/api.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/api.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/authorizer.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/authorizer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/domain_name.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/domain_name.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/integration.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/integration.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/route.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/route.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/stage.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/stage.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/apigatewayv2/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/apigatewayv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/application_autoscaling/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/application_autoscaling/scalable_target.py` & `idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scalable_target.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/application_autoscaling/scaling_policy.py` & `idem-aws-1.7.5/idem_aws/tool/aws/application_autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/arn_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/arn_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/auto_scaling_group_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/scaling_policy.py` & `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/scaling_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/autoscaling/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/autoscaling/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/backup/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/backup/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/backup/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/backup/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/budgets/budget.py` & `idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/budgets/budget_action.py` & `idem-aws-1.7.5/idem_aws/tool/aws/budgets/budget_action.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/budgets/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/budgets/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudformation/stack.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/cloudfront_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/cloudfront_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/distribution.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     timeout: Dict[str, Any],
 ):
     result = dict(comment=(), result=True, ret=None)
     # cloudfront distribution requires all params to be sent for update call even though one parameter change.
     # we will check if at least one attribute is changed and send the update request if any of the attribute changes.
 
     update_allowed_params = [
-        "caller_reference",
         "origins",
         "default_cache_behaviour",
         "comment",
         "logging",
         "enabled",
         "viewer_certificate",
         "aliases",
@@ -57,15 +56,20 @@
 
     modified_params = {}
     for parameter in update_allowed_params:
         if locals()[parameter] is not None:
             if isinstance(locals()[parameter], List) or isinstance(
                 locals()[parameter], Dict
             ):
-                if data.recursive_diff(before.get(parameter), locals()[parameter]):
+                if data.recursive_diff(
+                    before.get(parameter),
+                    locals()[parameter],
+                    ignore_order=True,
+                    ignore_missing_keys=True,
+                ):
                     modified_params[parameter] = locals()[parameter]
             elif before.get(parameter) != locals()[parameter]:
                 modified_params[parameter] = locals()[parameter]
 
     if modified_params:
         result["ret"] = modified_params
         if not ctx.get("test", False):
```

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/distribution_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/distribution_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudfront/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudfront/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudtrail/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudtrail/trail.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/log_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/log_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/metric_alarm.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/metric_alarm.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudwatch/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatch/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/cloudwatchlogs/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/comment_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/comment_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,21 @@
     return (f"Would delete {resource_type} '{name}'",)
 
 
 def already_absent_comment(hub, resource_type: str, name: str) -> Tuple:
     return (f"{resource_type} '{name}' already absent",)
 
 
+def missing_args_for_absent_comment(
+    hub, resource_type: str, name: str, args: list
+) -> Tuple:
+    n = "is" if len(args) == 1 else "are"
+    return (f"{args} {n} required to delete {resource_type} '{name}'",)
+
+
 def already_exists_comment(hub, resource_type: str, name: str) -> Tuple:
     return (f"{resource_type} '{name}' already exists",)
 
 
 def update_tags_comment(hub, tags_to_remove, tags_to_add) -> Tuple:
     return (f"Update tags: Add {tags_to_add} Remove {tags_to_remove}",)
 
@@ -92,8 +99,10 @@
         f"Update options for {resource_type} resource with name - {name} and id - {resource_id}",
     )
 
 
 def invalid_parameter_provided_comment(
     hub, parameter_name: str, resource_type: str, name: str
 ) -> Tuple:
-    return f"Invalid {parameter_name} was provided for resource type - {resource_type} with name - {name}"
+    return (
+        f"Invalid {parameter_name} was provided for resource type - {resource_type} with name - {name}",
+    )
```

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/config/config_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/config/config_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/config/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/config/delivery_channel.py` & `idem-aws-1.7.5/idem_aws/tool/aws/config/delivery_channel.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/config/rule.py` & `idem-aws-1.7.5/idem_aws/tool/aws/config/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/config/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/config/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/anomaly_monitor.py` & `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_monitor.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/anomaly_subscription.py` & `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/anomaly_subscription.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/costexplorer/cost_category.py` & `idem-aws-1.7.5/idem_aws/tool/aws/costexplorer/cost_category.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/docdb/db_cluster.py` & `idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/docdb/db_subnet_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/docdb/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/docdb/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/docdb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/dynamodb/table.py` & `idem-aws-1.7.5/idem_aws/tool/aws/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/ami.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/ami.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/availability_zones.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/dhcp_option_association_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/elastic_ip.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/flow_log.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/flow_log.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/data.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/key_pair.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/state.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/state.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/block_device_mappings.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/bootstrap.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/contracts/init.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/disable_api_termination.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ebs_optimized.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/iam_instance_profile_arn.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/init.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/init.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_initiated_shutdown_behavior.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/instance_type.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/instance_type.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/kernel_id.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/kernel_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/placement.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/placement.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/private_ip_address.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/ram_disk_id.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/security_group_ids.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/source_dest_check.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/sriov_net_support.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/tags.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/tags.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/instance/update/user_data.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/instance/update/user_data.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/internet_gateway.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/internet_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/key_pair.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/key_pair.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/launch_template.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/launch_template.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/network_interface.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/network_interface.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/placement_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/placement_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/route_table.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/route_table.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/security_group_rule.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/snapshot.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/spot_instance_request.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/spot_instance_request.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/subnet.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/transit_gateway.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/volume.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/vpc.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/vpc_endpoint.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ec2/vpc_peering_connection_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ecr/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ecr/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ecr/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ecr/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/efs/file_system_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/efs/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/efs/mount_target_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/efs/mount_target_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/efs/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/efs/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/eks/addon.py` & `idem-aws-1.7.5/idem_aws/tool/aws/eks/addon.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/eks/cluster.py` & `idem-aws-1.7.5/idem_aws/tool/aws/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/eks/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/eks/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/eks/eks_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/eks/eks_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/eks/nodegroup.py` & `idem-aws-1.7.5/idem_aws/tool/aws/eks/nodegroup.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/eks/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/eks/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elasticache/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elasticache/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elasticache/elasticache_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elasticache/elasticache_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elasticache/parameters.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elasticache/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elb/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elb/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elb/load_balancer.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elb/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elb/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elbv2/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elbv2/listener.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/listener.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elbv2/load_balancer.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/load_balancer.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elbv2/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/elbv2/target_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/elbv2/target_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/es/elasticsearch_domain.py` & `idem-aws-1.7.5/idem_aws/tool/aws/es/elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/es/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/es/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/events/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/events/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/events/rule.py` & `idem-aws-1.7.5/idem_aws/tool/aws/events/rule.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/events/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/events/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/guardduty/config_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/guardduty/config_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/guardduty/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/guardduty/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/guardduty/detector.py` & `idem-aws-1.7.5/idem_aws/tool/aws/guardduty/detector.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/group_membership.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/group_membership.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/password_policy.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/password_policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/policy.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/policy.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/role_policy_attachment.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/role_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/service_linked_role.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/service_linked_role.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/user.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/user.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/iam/user_ssh_key.py` & `idem-aws-1.7.5/idem_aws/tool/aws/iam/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/kinesis/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/kinesis/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/kinesis/stream.py` & `idem-aws-1.7.5/idem_aws/tool/aws/kinesis/stream.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/kinesis/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/kinesis/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/kms/alias.py` & `idem-aws-1.7.5/idem_aws/tool/aws/kms/alias.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/kms/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/kms/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/kms/key.py` & `idem-aws-1.7.5/idem_aws/tool/aws/kms/key.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/kms/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/kms/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function.py` & `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py` & `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_event_invoke_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function_permission.py` & `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_permission.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py` & `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/function_provisioned_concurrency_config.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/lambda_aws/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/lambda_aws/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/logs/subscription_filter_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/logs/subscription_filter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/neptune/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/neptune/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_cluster.py` & `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_cluster_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_instance.py` & `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_instance.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_parameter_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/neptune/db_subnet_group.py` & `idem-aws-1.7.5/idem_aws/tool/aws/neptune/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/neptune/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/neptune/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/network_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/network_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/organizations/account.py` & `idem-aws-1.7.5/idem_aws/tool/aws/organizations/account.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/organizations/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/organizations/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/organizations/policy_attachment.py` & `idem-aws-1.7.5/idem_aws/tool/aws/organizations/policy_attachment.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/organizations/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/organizations/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/parameters.py` & `idem-aws-1.7.5/idem_aws/tool/aws/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/rds/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/rds/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/rds/parameters.py` & `idem-aws-1.7.5/idem_aws/tool/aws/rds/parameters.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/route53/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/route53/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/route53/hosted_zone_association.py` & `idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_association.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/route53/hosted_zone_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/route53/hosted_zone_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/route53/resource_record_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/route53/resource_record_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/route53/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/route53/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_acl.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_encryption.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_lifecycle.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_logging.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_logging.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_replication.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_replication.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_versioning.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/bucket_website.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/bucket_website.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/s3/s3_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/search_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/search_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/ses/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/ses/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/sesv2/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/sesv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/sns/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/sns/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/sns/sns_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/sns/sns_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/sqs/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/sqs/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/sqs/queue_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/sqs/queue_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/state_comparison_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/state_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/string_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/string_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/tag_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/tag_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/test_state_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/wafv2/conversion_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/wafv2/ip_set_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/ip_set_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/wafv2/regex_pattern_set.py` & `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/regex_pattern_set.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/wafv2/tag.py` & `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/tag.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/wafv2/web_acl.py` & `idem-aws-1.7.5/idem_aws/tool/aws/wafv2/web_acl.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/aws/waiter_utils.py` & `idem-aws-1.7.5/idem_aws/tool/aws/waiter_utils.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/boto3/client.py` & `idem-aws-1.7.5/idem_aws/tool/boto3/client.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/boto3/custom_waiter.py` & `idem-aws-1.7.5/idem_aws/tool/boto3/custom_waiter.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/boto3/region.py` & `idem-aws-1.7.5/idem_aws/tool/boto3/region.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/boto3/resolve.py` & `idem-aws-1.7.5/idem_aws/tool/boto3/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/boto3/resource.py` & `idem-aws-1.7.5/idem_aws/tool/boto3/resource.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/boto3/session.py` & `idem-aws-1.7.5/idem_aws/tool/boto3/session.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws/tool/heist/bootstrap.py` & `idem-aws-1.7.5/idem_aws/tool/heist/bootstrap.py`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws.egg-info/PKG-INFO` & `idem-aws-1.7.5/idem_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-aws
-Version: 1.7.4
+Version: 1.7.5
 Summary: AWS Cloud Provider for Idem
 Home-page: https://docs.idemproject.io/idem-aws/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-aws
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-aws/issues
```

### Comparing `idem-aws-1.7.4/idem_aws.egg-info/SOURCES.txt` & `idem-aws-1.7.5/idem_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-aws-1.7.4/idem_aws.egg-info/requires.txt` & `idem-aws-1.7.5/idem_aws.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 acct<9.0.0,>=8.3.3
-boto3<1.25.0,>=1.24.0
+boto3<1.27.0,>=1.25.0
 configparser<6.0.0,>=5.0.0
 idem<22.0.0,>=20.7.0
 pgpy<0.6.0,>=0.5.4
 deepdiff<6.0.0,>=5.8.0
 heist<7.0.0,>=6.1.0
 pycryptodomex<3.14.0,>=3.10
 pop-serial<2.0.0,>=1.1.0
@@ -15,24 +15,24 @@
 textwrap3
 tqdm
 
 [bootstrap]
 heist-salt<6.0.0,>=5.3.1
 
 [full]
+localstack
+msgpack
 localstack-client
 pop-create-idem==2.0.4
-localstack
+textwrap3
 tqdm
-heist-salt<6.0.0,>=5.3.1
 localstack-ext
+heist-salt<6.0.0,>=5.3.1
 aws-google-auth>=0.0.35
 inflect
-msgpack
-textwrap3
 
 [google_auth]
 aws-google-auth>=0.0.35
 msgpack
 
 [localstack]
 localstack
```

### Comparing `idem-aws-1.7.4/setup.py` & `idem-aws-1.7.5/setup.py`

 * *Files identical despite different names*

