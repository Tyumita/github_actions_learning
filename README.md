# Github Actions について

## 概要
GitHub Actions は、ビルド、テスト、デプロイのパイプラインを自動化できる継続的インテグレーションと継続的デリバリー (CI/CD) のプラットフォームです。
リポジトリに対するすべての pull request をビルドしてテストしたり、マージされた pull request を運用環境にデプロイしたりするワークフローを作成できます。

GitHub Actions は、DevOps であるだけでなく、リポジトリで他のイベントが発生したときにワークフローを実行できます。
たとえば、リポジトリで新しい issue が作成されるたびに、適切なラベルを自動的に追加するワークフローを実行できます。

GitHub では、ワークフローを実行するための Linux、Windows、macOS 仮想マシンが提供されます。
また、自身のデータセンターまたはクラウド インフラストラクチャで独自のセルフホスト ランナーをホストすることもできます。

## CI\CDについて
### CI（Continuous Integration）
CIはContinuous Integrationの略で日本語では「継続的インティグレーション」と呼ばれています。

ソフトウェア開発における品質管理を短期間で行う手法のことで、実際には、頻繁に繰り返しビルドを実行するといった作業を行っています。
開発効率化や問題の早期発見などが可能になることがメリットですが、開発サイクルを短期間で回すため、コストが高くついてしまうのが難点。

そのため、CIを導入する場合には、多くの作業を自動化してくれる「CIツール」が採用されています。
「Circle CI」や「Jenkins」などのツールが有名どころです。

### CD（Continuous Delivery・Continuous Deployment）
CDは日本語で「継続的デリバリー」や「継続的デプロイメント」などと呼ばれています。

継続的デリバリーとは、開発者によるコード変更に対して、バグがないか自動的にテストし、実稼働環境へのリリース準備が実行される手法のこと。
それに対し、断続的デプロイメントとは、断続的デリバリーのプロセスをさらに延長して、自動的に本番環境にリリースした後、顧客が使用できるようにするというものです。

厳密にはどちらも異なる手法すが、同じ意味として使用されてることもあるようです。