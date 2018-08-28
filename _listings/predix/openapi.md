swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/catalog/artifacts/{id}/file:
    get:
      summary: Download an artifact file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadAnalyticArtifact
      x-api-path-slug: apiv1catalogartifactsidfile-get
      parameters:
      - in: path
        name: id
        description: artifact id
      responses:
        2:
          description: Successful response
      tags:
      - Download
      - Artifact
      - File
      - By
      - Id
  /api/v2/config/orchestrations/artifacts/{id}/file:
    get:
      summary: Download an orchestration artifact file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadOrchConfigArtifact
      x-api-path-slug: apiv2configorchestrationsartifactsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Artifact id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Download
      - Orchestration
      - Artifact
      - File
      - By
      - Id
  /api/v2/config/orchestrations/models/{id}/file:
    get:
      summary: Download a model file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadModel
      x-api-path-slug: apiv2configorchestrationsmodelsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: Model id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Download
      - Model
      - File
      - By
      - Id
  /api/v2/config/orchestrations/{id}/file:
    get:
      summary: Download an orchestration artifact file by orchestration id and artifact
        type.
      description: The file is downloaded as an octet-stream. If the type is bpmn,
        then then bpmn xml is downloaded. If the type is portToFieldMap, then the
        system expects analyticStepId to download the portToFieldMap for the given
        step
      operationId: downloadArtifactByType
      x-api-path-slug: apiv2configorchestrationsidfile-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
        description: orchestration configuration entry id
      - in: query
        name: name
        description: artifact name (analytic step id)
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: type
        description: artifact type (Ex
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Download
      - Orchestration
      - Artifact
      - File
      - By
      - Orchestration
      - Id
      - Artifact
      - Type
  /api/v2/execution/orchestrations/{orchConfigId}/deployment:
    post:
      summary: Deploy the specified orchestration workflow file to the Orchestration
        Engine.
      description: This API will deploy the BPMN file associated with the specified
        orchestration configuration to the Orchestration Engine in preparation for
        orchestration execution.
      operationId: retrieveAndDeployBpmn
      x-api-path-slug: apiv2executionorchestrationsorchconfigiddeployment-post
      parameters:
      - in: path
        name: orchConfigId
        description: orchestration configuration id
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Deploy
      - Specified
      - Orchestration
      - Workflow
      - File
      - To
      - Orchestration
      - Engine