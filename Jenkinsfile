@Library('libpipelines@master') _

hose {
    EMAIL = 'clouds-integration@stratio.com'
    BUILDTOOL = 'make'
    VERSIONING_TYPE = 'stratioVersion-3-3'
    UPSTREAM_VERSION = '1.6.0'
    DEPLOYONPRS = true
    DEVTIMEOUT = 30
    ANCHORE_POLICY = "production"
    GRYPE_TEST = false

    BUILDTOOL_MEMORY_REQUEST = "1024Mi"
    BUILDTOOL_MEMORY_LIMIT = "4096Mi"

    DEV = { config ->
        doDocker(conf:config, dockerfile: 'Dockerfile', image:'cluster-api-provider-gcp')
    }
}
