# helm-repo-add-release-agent-https-circleci-public.github.io-cci-k8s-release-agent
:electron: Build cross-platform desktopps with JavaScript, HTML, and CSS
helm repo add release-agent https://circleci-public.github.io/cci-k8s-release-agent
helm upgrade --install circleci-release-agent-system release-agent/circleci-release-agent \
    --set tokenSecret.token=CCIRIT_AGgidDZvofLXdEyTfz5ffC_44b5e39f87594984a18bd70838c8679ad7cf2b97 \
    --create-namespace \
    --namespace circleci-release-agent-system \
    --set managedNamespaces="{default}"
    helm repo update
    https://circleci-public.github.io/cci-k8s-release-agent
