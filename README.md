A handy lookup table of similar technology and services to help ex-googlers survive the *real* world :)
pull-requests very welcomed. __Please do not list any confidential projects!__

For a working example of (some) of these technologies integrated together, see:
https://github.com/google/startup-os

See also: [System Design Primer](https://github.com/donnemartin/system-design-primer), [The Hadoop Ecosystem Table](https://hadoopecosystemtable.github.io/), [Map AWS services to GCP products](https://cloud.google.com/free/docs/map-aws-google-cloud-platform)

## Technology

### Core Technology

| Google Internal | Google External                          | Open Source / Real-World                 |
| --------------- | ---------------------------------------- | ---------------------------------------- |
| MapReduce       |                                          | [Apache Hadoop](https://github.com/apache/hadoop), [Spark](https://github.com/apache/spark) |
| Protocol Buffer | [Protobuf](https://github.com/google/protobuf) | [Cap'n Proto](https://capnproto.org/), [Thrift](https://github.com/apache/thrift), [Avro](https://github.com/apache/avro), [Amazon Ion](https://amzn.github.io/ion-docs/), [CBOR](https://cbor.io/) |
| Stubby          | [gRPC](https://github.com/grpc/grpc)     | [Thrift](https://github.com/apache/thrift), [Bolt](https://boltprotocol.org/) |
| Chubby          |                                          | [Apache Zookeeper](https://github.com/apache/zookeeper), [etcd](https://github.com/coreos/etcd), [HashiCorp Consul](https://github.com/hashicorp/consul) |
| Goops / PubSub  |                                          | [Apache Kafka](https://github.com/apache/kafka), [Apache Pulsar](https://github.com/apache/incubator-pulsar), [Facebook LogDevice](https://github.com/facebookincubator/LogDevice) |


### Infrastructure

| Google Internal      | Google External                          | Open Source / Real-World                 |
| -------------------- | ---------------------------------------- | ---------------------------------------- |
| Borg                 |                                          | [Kubernetes](https://kubernetes.io/), [Apache Mesos](https://github.com/apache/mesos), [HashiCorp Nomad](https://github.com/hashicorp/nomad) |
| GSLB, GFE, Maglev    |                                          | ELB, [HAProxy](http://www.haproxy.org/), [Istio](https://istio.io/), [F5](https://f5.com/products/big-ip), [envoy](https://github.com/lyft/envoy) |
| data center hardware | [open compute](http://www.opencompute.org/) |                                          |
| Jupiter, Starblaze   |                                          |                                             |
| B4, Stargate, TE     |                                          |                                             |
| USPS, Andromeda      |                                          |                                             |


### Storage

| Google Internal                          | Google External                          | Open Source / Real-World                 |
| ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| GFS/Colossus                             |                                          | HDFS, [Ceph](https://ceph.com), [GlusterFS](https://www.gluster.org) |
| BigTable                                 | [Cloud BigTable](https://cloud.google.com/bigtable) | [PrestoDB](https://prestodb.io/), [Cassandra](https://github.com/apache/cassandra), [HBase](https://github.com/apache/hbase), [Accumulo](https://github.com/apache/accumulo), [DynamoDB](https://aws.amazon.com/dynamodb), [ScyllaDB](https://www.scylladb.com/) |
| [Spanner](http://research.google.com/archive/spanner.html) | [Cloud Spanner](https://cloud.google.com/spanner/) | [Vitess](https://vitess.io), [CockroachDB](https://github.com/cockroachdb/cockroach), [TiDB](https://github.com/pingcap/tidb) |
| ColumnIO / [Capacitor](https://cloud.google.com/blog/big-data/2016/04/inside-capacitor-bigquerys-next-generation-columnar-storage-format) |                                          | [Apache Parquet](http://parquet.apache.org) |
| sstable                                  | [levelDB](https://github.com/google/leveldb) | [RocksDB](https://rocksdb.org)           |
| zippy                                    | [Snappy](https://github.com/google/snappy) | [lz4](https://github.com/lz4/lz4)        |


### Services
| Google Internal                          | Google External                          | Open Source                              | SaaS                                     |
| ---------------------------------------- | ---------------------------------------- | ---------------------------------------- | ---------------------------------------- |
| Dremel                                   | [BigQuery](https://cloud.google.com/bigquery/) | Apache Drill, [Presto](https://prestodb.io), Spark(sort-of), | AWS Athena, [Redshift Spectrum](https://aws.amazon.com/redshift/spectrum/) |
| Dremel UI                                |                                          | [Redash](https://github.com/getredash/redash), [Metabase](https://github.com/metabase/metabase), [Apache Superset](https://github.com/apache/incubator-superset) |                                          |
| Search (Mustang, Alexandria)             |                                          | Elasticsearch, Solr, Lucene              | [algolia](https://www.algolia.com/)      |
| pubsub                                   | [pubsub](https://cloud.google.com/pubsub/docs/overview) | [NATS.io](https://nats.io), RabbitMQ, [PubNub](https://www.pubnub.com/) | AWS SQS/SNS, [AWS AppSync](https://aws.amazon.com/appsync) |
| [Flume (Java)](https://ai.google/research/pubs/pub35650) | [Apache Beam](https://beam.apache.org/)  | [Apache Crunch](https://crunch.apache.org/) |                                          |
| [MillWheel](https://ai.google/research/pubs/pub41378) | [Cloud Dataflow](https://cloud.google.com/dataflow/) | [Apache Flink](https://flink.apache.org/) |                |

### DevOps
| Google Internal                 | Google External                          | Real-World                               |
| ------------------------------- | ---------------------------------------- | ---------------------------------------- |
| Assimilator                     |                                          | [Dominator](https://github.com/Symantec/Dominator) |
| Blaze                           | [Bazel](https://bazel.build)             | [Buck](https://buckbuild.com/), [Pants](https://www.pantsbuild.org/), [please.build](https://please.build/), [Blade](https://github.com/chen3feng/blade-build), [recc](https://gitlab.com/bloomberg/recc) |
| Oncall                          |                                          | [PagerDuty](https://pagerduty.com), [OpsGenie](https://www.opsgenie.com/), [VictorOps](https://victorops.com/) |
| varz/borgmon/monarch            |                                          | [Datadog](https://www.datadoghq.com/), [Prometheus](https://prometheus.io), [librato](https://www.librato.com), [newrelic](http://newrelic.com), skylight, scout, [Scotty](https://github.com/Symantec/scotty)/[tricorder](https://github.com/Symantec/tricorder), also [this](https://vimeo.com/173610242) and [this](https://prometheus.io/docs/introduction/comparison/) |
| Exception/Error Tracking (??)   |                                          | Sentry.io, Raygun.io, [Rollbar](https://rollbar.com), Honeybadger, Airbrake, OverOps |
| styleguides                     | [google styleguides](https://github.com/google/styleguide) | [PEP-8](https://www.python.org/dev/peps/pep-0008/), [HoundCI auto-style-reviewer](https://houndci.com/) |
| Blaze/Forge/TAP/BuildCop        | [Cloud Build](https://cloud.google.com/cloud-build/) | [buildkite](https://buildkite.com/), [CircleCI](https://circleci.com), [travis](https://travis-ci.org/), [jenkins](https://jenkins.io/), [gitlabCI](https://about.gitlab.com/product/continuous-integration/) |
| Sandman(test env)/Guitar        |                                          |                   |
| Sisyphus / Rapid                |                                          | [Spinnaker](https://www.spinnaker.io/), [lambdaCD](http://www.lambda.cd), screwdriver.cd, [CodeShip](https://codeship.com), [shipit-engine](https://github.com/Shopify/shipit-engine), [GoCD](https://www.gocd.org), [AWS CodeDeploy](https://aws.amazon.com/codedeploy/), [Capistrano](http://www.capistranorb.com), [Fabric](http://www.fabfile.org), [ConcourseCI](https://concourse.ci/) |
| borg / borgcfg / gcl            |                                          | [AWS Cloudformation](https://aws.amazon.com/cloudformation/), Puppet, Chef, Salt, Ansible, [Terraform](https://www.terraform.io), [Jsonnet](http://jsonnet.org/), [kubecfg](https://github.com/bitnami/kubecfg) |
| logging                         | [StackDriver](https://cloud.google.com/stackdriver/) | logstash, fluentd, papertrail, [cernan](https://github.com/postmates/cernan) |
| CodeSearch                      | [Zoekt](https://github.com/google/zoekt) | [Sourcegraph](https://sourcegraph.com), [OpenGrok](https://github.com/OpenGrok/OpenGrok/) |
| Critique, Gerrit, Mondrian etc. | [Gerrit](https://www.gerritcodereview.com/) | [Reviewable](https://reviewable.io) , [Phabricator](https://www.phacility.com/phabricator/)     |
| cider                           |                                          | [Eclipse Che](https://www.eclipse.org/che/), [Cloud9](https://c9.io/), [gitpod.io](https://gitpod.io), [Coder](https://coder.com/), [Code-Server (VSCode in a Tab)](https://github.com/cdr/code-server)|
| buganizer                       |                                          | [JIRA](https://www.atlassian.com/software/jira), [bugzilla](https://www.bugzilla.org/), github issues |
| ToTT                            | [Google Test Blog](https://testing.googleblog.com/) |                                          |
| Copybara / MOE                  | [Copybara](https://github.com/google/copybara), [MOE](https://github.com/google/MOE)  |                                          |
| workflow/dependency management | | luigi, airflow, digdag, packyderm, dask |
| ErrorProne                      | [ErrorProne](https://errorprone.info/)   | [SpotBugs](https://spotbugs.github.io/), [FindBugs](http://findbugs.sourceforge.net/) |
| dapper (distributed trace) | [stackdriver trace](https://cloud.google.com/trace/) | [zipkin](https://github.com/openzipkin/zipkin), [opentracing](https://opentracing.io/docs/overview/), [jaeger](https://www.jaegertracing.io/) |

### Security
| Google Internal                  | Google External | Open Source                              |
| -------------------------------- | --------------- | ---------------------------------------- |
| prodaccess/LOAS                  |                 | [Keymaster](https://github.com/Symantec/keymaster) |
| prod secrets/identity management |                 | [chamber](https://github.com/segmentio/chamber), [knox](https://github.com/pinterest/knox), [SPIFFE](https://spiffe.io/) |

## IT / Operations
| Google Internal                          | Real-World                               |
| ---------------------------------------- | ---------------------------------------- |
| [software engineering at google](https://arxiv.org/ftp/arxiv/papers/1702/1702.01715.pdf) |                                          |
| valentine                                | [1Password](https://support.1password.com/create-share-vaults/), [Lastpass](http://lastpass.com), [pass](https://www.passwordstore.org/) |
| OWNERS files in repo                     | [github CODEOWNERS](https://github.com/blog/2392-introducing-code-owners) |
| snippets                                 | [Khan/snippets](https://github.com/Khan/snippets) |
| memegen                                  | [memegen](http://www.memegen.com/)       |
| SnipIt                                   | [recordit](http://recordit.co/), [CloudApp](https://www.getcloudapp.com/), [dropbox screenshots](https://help.dropbox.com/installs-integrations/photos/screenshots) |
| edge, people ops training                | [LifeLabs](http://lifelabsnewyork.com/)  |
| googlegeist                              | [Culture Amp](https://www.cultureamp.com/), [humu](http://www.humu.com/), [tinypulse](https://www.tinypulse.com/), [peakon](https://peakon.com/) |
| HRIS/ERP                                 | [Namely](https://namely.com), [BambooHR](https://www.bamboohr.com/), [Workday](https://workday.com) |
| stuff (SaaS IT management)               | [intello](https://www.intello.io/), [zylo](https://zylo.com/) |
| stuff (Device Management)                | [Fleetsmith](https://www.fleetsmith.com/), [jamf](https://www.jamf.com/), [rippling IT](https://www.rippling.com/it/) |
| device security monitoring               | [Red Canary](https://redcanary.com/) |
| [go/ links](https://medium.com/@golinks/the-full-history-of-go-links-and-the-golink-system-cbc6d2c8bb3)                                | [golinks](https://www.golinks.io/), [go](https://github.com/kellegous/go), [Goat](https://goatcodes.com/) |
| google3 philosophy                       | [innersource](https://resources.github.com/whitepapers/introduction-to-innersource/), [monorepo](https://cacm.acm.org/magazines/2016/7/204032-why-google-stores-billions-of-lines-of-code-in-a-single-repository/fulltext) |
| safely sharing 1-time secrets            | [croc](https://github.com/schollz/croc), [onetimesecret](https://github.com/onetimesecret/onetimesecret), [privatebin](https://privatebin.info/) |
| messaging                                | [mattermost](https://github.com/mattermost/mattermost-server), slack, gchat |

also check out [xoogler.co](http://xoogler.co/), which organizes events, slack channels etc

*disclaimer: I'm not affiliated with any of the technologies mentioned above.*

*disclaimer: I left Google a number of years ago so some of the naming might be dated*
