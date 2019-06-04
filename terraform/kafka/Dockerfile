FROM kostyrev/hashicorp-terraform:0.11.14

ARG TERRAFORM_KAFKA_VERSION

RUN curl -sSL  https://github.com/Mongey/terraform-provider-kafka/releases/download/v${TERRAFORM_KAFKA_VERSION}/terraform-provider-kafka_${TERRAFORM_KAFKA_VERSION}_linux_amd64.tar.gz | tar xz \
    && mkdir -pv ~/.terraform.d/plugins \
    && mv terraform-provider-kafka ~/.terraform.d/plugins
