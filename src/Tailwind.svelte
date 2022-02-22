<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;

  @layer base {
    button {
      @apply bg-gray-200 hover:bg-gray-400 px-2 py-1.5;
    }

    input {
      @apply border rounded px-1 py-0.5;
    }

    a {
      @apply hover:underline text-blue-800;
    }

    ul {
      @apply list-disc list-inside;
    }

    @media screen {
      body {
        @apply bg-teal-100;
      }
    }
  }

  @layer components {
    @font-face {
      font-family: Inter;
      src: url('/static/font/Inter-Regular.otf');
    }

    @font-face {
      font-family: Inter;
      font-weight: bold;
      src: url('/static/font/Inter-Bold.otf');
    }

    @font-face {
      font-family: Inter;
      font-style: italic;
      src: url('/static/font/Inter-Italic.otf');
    }

    @font-face {
      font-family: Inter;
      font-weight: 300;
      src: url('/static/font/Inter-Light.otf');
    }

    @font-face {
      font-family: Inter;
      font-weight: bold;
      font-style: italic;
      src: url('/static/font/Inter-BoldItalic.otf');
    }
  }
</style>