サイトが独立プロジェクトなら、サイトのソースコードを保存するために新しいリポジトリを作成できます。 If your site is associated with an existing project, you can add the source code {% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.22" or currentVersion == "github-ae@latest" %}to that project's repository, in a `/docs` folder on the default branch or on a different branch.{% else %}for your site to a `gh-pages` branch or a `docs` folder on the `master` branch in that project's repository.{% endif %} For example, if you're creating a site to publish documentation for a project that's already on {% data variables.product.product_name %}, you may want to store the source code for the site in the same repository as the project.

{% if currentVersion == "free-pro-team@latest" %}If the account that owns the repository uses {% data variables.product.prodname_free_user %} or {% data variables.product.prodname_free_team %}, the repository must be public.{% endif %}

既存のリポジトリにサイトを作成したいのなら、[サイトの作成](#creating-your-site)セクションまでスキップしてください。