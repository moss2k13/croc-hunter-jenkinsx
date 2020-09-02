你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
# Croc Hunter - The game!

For those that have dreamt to hunt crocs

# Usage

Basic go webserver to demonstrate example CI/CD pipeline using Kubernetes

# Deploy using JenkinsX (Kubernetes, Helm, Monocular, ChartMuseum)

Just follow the [JenkinsX](http://jenkins-x.io) installation

For example, if using GKE with cert-manager preinstalled for https certificates

    jx install --provider=gke --domain=example.com --http=false --tls-acme=true

Then fork this repo and [import it](http://jenkins-x.io/developing/import/)

    jx import --url https://github.com/GITHUB_USER/croc-hunter-jenkinsx

Then, any PRs against this repo will be automatically deployed to preview environments.
When they are merged they will be deployed to the `staging` environment.

To [promote from staging to production](http://jenkins-x.io/developing/promote/) just run

    jx promote croc-hunter-jenkinsx --version 0.0.1 --env production

Then delete the PR environments

    jx delete env

# Acknowledgements

Original work by [Lachlan Evenson](https://github.com/lachie83/croc-hunter)
Continuation of the awesome work by everett-toews.
* https://gist.github.com/everett-toews/ed56adcfd525ce65b178d2e5a5eb06aa

## Watch Their Demo

https://www.youtube.com/watch?v=eMOzF_xAm7w
