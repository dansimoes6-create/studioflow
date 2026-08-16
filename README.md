# StudioFlow — Gestão Criativa

Aplicativo mobile para uma empresa de edição de vídeo, design, sites e aplicativos.

## Recursos

- Painel com faturamento, despesas, saldo e valores a receber
- Cadastro de clientes
- Projetos com serviço, valor, status e progresso
- Lançamentos financeiros de entradas e saídas
- Exportação financeira em CSV
- Dados salvos offline no aparelho
- Layout responsivo, instalável como PWA

## Gerar o APK Android

Com Node.js, Java JDK 17 e Android Studio/SDK instalados:

```bash
npm install
npm run android:init
npm run android:sync
npm run android:apk
```

O APK de teste será criado em `android/app/build/outputs/apk/debug/app-debug.apk`.

Para testar no navegador, abra `index.html` por um servidor local (`npm start`).

## Gerar apenas pelo celular com GitHub Actions

1. Crie uma conta em github.com pelo navegador do celular.
2. Crie um repositório novo, descompacte este arquivo e envie todos os arquivos para ele (inclusive a pasta `.github`).
3. Abra a aba **Actions** do repositório e toque em **Build APK** > **Run workflow**.
4. Quando a execução terminar, abra-a e baixe o arquivo em **Artifacts** com o nome `StudioFlow-debug-apk`.
