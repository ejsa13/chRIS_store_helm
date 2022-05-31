# chRIS_store_helm
helm charts for chRIS store backend and ui.

postgres and swift are dependency chart for the chRIS store backend. If deploying in OCP, serviceaccounts for postgres (postres-sa), swift (swift-sa) and chRIS should have "anyuid" scc on it. The backend and fronted uses the same service account.

Images are stored in quay.io/chrisproject

chRIS_store was built using the Docker file in fnndsc/chRIS_store github repository. The chRIS_store_ui was build using the Docker file in fnndsc/chRIS_store_ui github repository but the .env was excluded in the docker build.