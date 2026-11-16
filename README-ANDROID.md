# Lutas Brasileiras — Android APK

Projeto Android nativo (WebView local) que empacota a aplicação educativa em APK. O conteúdo web é incluído em `app/src/main/assets/www`, portanto o jogo e as imagens são carregados localmente.

## Gerar o APK
O workflow do GitHub Actions está em `.github/workflows/build-apk.yml`.

1. Crie um repositório GitHub e envie todos os arquivos desta pasta.
2. Abra a aba **Actions**.
3. Selecione **Gerar APK Android** e clique em **Run workflow** (ou aguarde o build após o push).
4. Quando terminar, abra a execução e baixe o artefato **Lutas-Brasileiras-APK**.
5. Extraia o ZIP do artefato: dentro estará `app-debug.apk`.
6. Transfira o APK para o Android e autorize a instalação de apps dessa origem, se solicitado.

## Requisitos
- Android 6.0 ou superior (minSdk 23).
- O APK debug é para instalação e testes; não é uma versão assinada para publicação na Play Store.
- Não usa backend nem serviços pagos. O jogo e os recursos incluídos funcionam localmente. Fontes remotas podem usar fontes substitutas quando não houver internet.

## Identificação
- Nome: Lutas Brasileiras
- Pacote: `br.com.lutasbrasileiras.quiz`
- Versão: 1.0.0
