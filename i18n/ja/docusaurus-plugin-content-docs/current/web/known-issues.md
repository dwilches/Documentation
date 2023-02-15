# 既知の問題

## v1.3.1
- ```DocumentExportOptions``` が使用されている場合、ヘッドレス エクスポートは失敗します。代わりにフォーマット固有のクラス (例: ```PdfExportOptions```) を使用してください。

## v1.3.0

- 散布図 / 階級区分図の表示形式は、プログラムによってエクスポートされたダッシュボードに表示されません。
- NuGet パッケージを使用する際に、Reveal SDK のライセンス (SDK インストーラーに有効なキーを入力) 後もウォーターマークが表示されてしまいます。

**回避策**: プロジェクトから NuGet パッケージをアンインストールし、NuGet のキャッシュをクリアして、パッケージを再度インストールしてください。NuGet のすべてのキャッシュをクリアしたくない場合、キャッシュした場所を検索し、Infragistics Reveal 項目のみをクリアできます。場所は NuGet のバージョンと、packages.config または PackageReferece のどちらが使用されているかによって異なります。