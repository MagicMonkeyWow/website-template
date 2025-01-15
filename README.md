# website-template
this is a website written by HTML which is made for testing Playful Old Citizen Game

            <html>
              
      <head>
        <script src="https://cdn.jsdelivr.net/npm/apexcharts"></script>
        <script src="https://cdn.tailwindcss.com"></script>
        <script>
            window.FontAwesomeConfig = {
                autoReplaceSvg: 'nest', // Options: 'nest', 'remove', 'replace'
            };
        </script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/js/all.min.js" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

      <style>
        * {
          font-family: "Inter", sans-serif;
        }

        ::-webkit-scrollbar {
          display: none;
        }

        .highlighted-section {
          outline: 2px solid #3F20FB;
          background-color: rgba(63, 32, 251, 0.1);
        }

        .edit-button {
          position: absolute;
          z-index: 1000;
        }

       :root {
          /* Base colors */
          --color-base: #ffffff;
          --color-base-50: #f9fafb;
          --color-base-100: #f3f4f6;
          --color-base-200: #e5e7eb;
          --color-base-300: #d1d5db;
          --color-base-400: #9ca3af;
          --color-base-500: #6b7280;
          --color-base-600: #4b5563;  
          --color-base-700: #374151;
          --color-base-800: #1f2937;  
          --color-base-900: #111827;
          --color-base-content: #1f2937;

          /* Primary colors */
          --color-primary: #3b82f6;
          --color-primary-50: #eff6ff;
          --color-primary-100: #dbeafe;
          --color-primary-200: #bfdbfe;
          --color-primary-300: #93c5fd;
          --color-primary-400: #60a5fa;
          --color-primary-500: #3b82f6;
          --color-primary-600: #2563eb;
          --color-primary-700: #1d4ed8;
          --color-primary-800: #1e40af;
          --color-primary-900: #1e3a8a;
          --color-primary-focus: #2563eb;
          --color-primary-content: #ffffff;

          /* Secondary colors */
          --color-secondary: #8b5cf6;
          --color-secondary-50: #f5f3ff;
          --color-secondary-100: #ede9fe;
          --color-secondary-200: #ddd6fe;
          --color-secondary-300: #c4b5fd;
          --color-secondary-400: #a78bfa;
          --color-secondary-500: #8b5cf6;
          --color-secondary-600: #7c3aed;
          --color-secondary-700: #6d28d9;
          --color-secondary-800: #5b21b6;
          --color-secondary-900: #4c1d95;
          --color-secondary-focus: #7c3aed;
          --color-secondary-content: #ffffff;

          /* Accent colors */
          --color-accent: #f472b6;
          --color-accent-50: #fdf2f8;
          --color-accent-100: #fce7f3;
          --color-accent-200: #fbcfe8;
          --color-accent-300: #f9a8d4;
          --color-accent-400: #f472b6;
          --color-accent-500: #ec4899;
          --color-accent-600: #db2777;
          --color-accent-700: #be185d;
          --color-accent-800: #9d174d;
          --color-accent-900: #831843;
          --color-accent-focus: #db2777;
          --color-accent-content: #ffffff;

          /* Neutral colors */
          --color-neutral: #6b7280;
          --color-neutral-50: #f9fafb;
          --color-neutral-100: #f3f4f6;
          --color-neutral-200: #e5e7eb;
          --color-neutral-300: #d1d5db;
          --color-neutral-400: #9ca3af;
          --color-neutral-500: #6b7280;
          --color-neutral-600: #4b5563;
          --color-neutral-700: #374151;
          --color-neutral-800: #1f2937;
          --color-neutral-900: #111827;
          --color-neutral-focus: #4b5563;
          --color-neutral-content: #ffffff;

          /* Info colors */
          --color-info: #3b82f6;
          --color-info-50: #eff6ff;
          --color-info-100: #dbeafe;
          --color-info-200: #bfdbfe;
          --color-info-300: #93c5fd;
          --color-info-400: #60a5fa;
          --color-info-500: #3b82f6;
          --color-info-600: #2563eb;
          --color-info-700: #1d4ed8;
          --color-info-800: #1e40af;
          --color-info-900: #1e3a8a;
          --color-info-focus: #2563eb;
          --color-info-content: #ffffff;

          /* Success colors */
          --color-success: #10b981;
          --color-success-50: #ecfdf5;
          --color-success-100: #d1fae5;
          --color-success-200: #a7f3d0;
          --color-success-300: #6ee7b7;
          --color-success-400: #34d399;
          --color-success-500: #10b981;
          --color-success-600: #059669;
          --color-success-700: #047857;
          --color-success-800: #065f46;
          --color-success-900: #064e3b;
          --color-success-focus: #059669;
          --color-success-content: #ffffff;

          /* Warning colors */
          --color-warning: #f59e0b;
          --color-warning-50: #fffbeb;
          --color-warning-100: #fef3c7;
          --color-warning-200: #fde68a;
          --color-warning-300: #fcd34d;
          --color-warning-400: #fbbf24;
          --color-warning-500: #f59e0b;
          --color-warning-600: #d97706;
          --color-warning-700: #b45309;
          --color-warning-800: #92400e;
          --color-warning-900: #78350f;
          --color-warning-focus: #d97706;
          --color-warning-content: #ffffff;

          /* Error colors */
          --color-error: #ef4444;
          --color-error-50: #fef2f2;
          --color-error-100: #fee2e2;
          --color-error-200: #fecaca;
          --color-error-300: #fca5a5;
          --color-error-400: #f87171;
          --color-error-500: #ef4444;
          --color-error-600: #dc2626;
          --color-error-700: #b91c1c;
          --color-error-800: #991b1b;
          --color-error-900: #7f1d1d;
          --color-error-focus: #dc2626;
          --color-error-content: #ffffff;
        }

        /* Dark theme */
        .dark {
          /* Base colors */
          --color-base: #1f2937;
          --color-base-50: #111827;
          --color-base-100: #1f2937;
          --color-base-200: #374151;
          --color-base-300: #4b5563;
          --color-base-400: #6b7280;
          --color-base-500: #9ca3af;
          --color-base-600: #d1d5db;
          --color-base-700: #e5e7eb;
          --color-base-800: #f3f4f6;
          --color-base-900: #f9fafb;
          --color-base-content: #f9fafb;

          /* Primary colors */
          --color-primary: #60a5fa;
          --color-primary-50: #1e3a8a;
          --color-primary-100: #1e40af;
          --color-primary-200: #1d4ed8;
          --color-primary-300: #2563eb;
          --color-primary-400: #3b82f6;
          --color-primary-500: #60a5fa;
          --color-primary-600: #93c5fd;
          --color-primary-700: #bfdbfe;
          --color-primary-800: #dbeafe;
          --color-primary-900: #eff6ff;
          --color-primary-focus: #3b82f6;
          --color-primary-content: #1f2937;

          /* Secondary colors */
          --color-secondary: #a78bfa;
          --color-secondary-50: #4c1d95;
          --color-secondary-100: #5b21b6;
          --color-secondary-200: #6d28d9;
          --color-secondary-300: #7c3aed;
          --color-secondary-400: #8b5cf6;
          --color-secondary-500: #a78bfa;
          --color-secondary-600: #c4b5fd;
          --color-secondary-700: #ddd6fe;
          --color-secondary-800: #ede9fe;
          --color-secondary-900: #f5f3ff;
          --color-secondary-focus: #8b5cf6;
          --color-secondary-content: #1f2937;

          /* Accent colors */
          --color-accent: #f472b6;
          --color-accent-50: #831843;
          --color-accent-100: #9d174d;
          --color-accent-200: #be185d;
          --color-accent-300: #db2777;
          --color-accent-400: #ec4899;
          --color-accent-500: #f472b6;
          --color-accent-600: #f9a8d4;
          --color-accent-700: #fbcfe8;
          --color-accent-800: #fce7f3;
          --color-accent-900: #fdf2f8;
          --color-accent-focus: #ec4899;
          --color-accent-content: #1f2937;

          /* Neutral colors remain the same as light theme */

          /* Info colors */
          --color-info: #60a5fa;
          --color-info-50: #1e3a8a;
          --color-info-100: #1e40af;
          --color-info-200: #1d4ed8;
          --color-info-300: #2563eb;
          --color-info-400: #3b82f6;
          --color-info-500: #60a5fa;
          --color-info-600: #93c5fd;
          --color-info-700: #bfdbfe;
          --color-info-800: #dbeafe;
          --color-info-900: #eff6ff;
          --color-info-focus: #3b82f6;
          --color-info-content: #1f2937;

          /* Success colors */
          --color-success: #34d399;
          --color-success-50: #064e3b;
          --color-success-100: #065f46;
          --color-success-200: #047857;
          --color-success-300: #059669;
          --color-success-400: #10b981;
          --color-success-500: #34d399;
          --color-success-600: #6ee7b7;
          --color-success-700: #a7f3d0;
          --color-success-800: #d1fae5;
          --color-success-900: #ecfdf5;
          --color-success-focus: #10b981;
          --color-success-content: #1f2937;

          /* Warning colors */
          --color-warning: #fbbf24;
          --color-warning-50: #78350f;
          --color-warning-100: #92400e;
          --color-warning-200: #b45309;
          --color-warning-300: #d97706;
          --color-warning-400: #f59e0b;
          --color-warning-500: #fbbf24;
          --color-warning-600: #fcd34d;
          --color-warning-700: #fde68a;
          --color-warning-800: #fef3c7;
          --color-warning-900: #fffbeb;
          --color-warning-focus: #f59e0b;
          --color-warning-content: #1f2937;

          /* Error colors */
          --color-error: #f87171;
          --color-error-50: #7f1d1d;
          --color-error-100: #991b1b;
          --color-error-200: #b91c1c;
          --color-error-300: #dc2626;
          --color-error-400: #ef4444;
          --color-error-500: #f87171;
          --color-error-600: #fca5a5;
          --color-error-700: #fecaca;
          --color-error-800: #fee2e2;
          --color-error-900: #fef2f2;
          --color-error-focus: #ef4444;
          --color-error-content: #1f2937;
        }
      </style>

      <script>
        tailwind.config = {
            theme: {
              extend: {
                colors: {
                  // Default Tailwind colors
                  transparent: 'transparent',
                  current: 'currentColor',
                  black: '#000000',
                  white: '#ffffff',
                  gray: {
                    50: '#f9fafb',
                    100: '#f3f4f6',
                    200: '#e5e7eb',
                    300: '#d1d5db',
                    400: '#9ca3af',
                    500: '#6b7280',
                    600: '#4b5563',
                    700: '#374151',
                    800: '#1f2937',
                    900: '#111827',
                  },
                  red: {
                    50: '#fef2f2',
                    100: '#fee2e2',
                    200: '#fecaca',
                    300: '#fca5a5',
                    400: '#f87171',
                    500: '#ef4444',
                    600: '#dc2626',
                    700: '#b91c1c',
                    800: '#991b1b',
                    900: '#7f1d1d',
                  },
                  yellow: {
                    50: '#fffbeb',
                    100: '#fef3c7',
                    200: '#fde68a',
                    300: '#fcd34d',
                    400: '#fbbf24',
                    500: '#f59e0b',
                    600: '#d97706',
                    700: '#b45309',
                    800: '#92400e',
                    900: '#78350f',
                  },
                  green: {
                    50: '#ecfdf5',
                    100: '#d1fae5',
                    200: '#a7f3d0',
                    300: '#6ee7b7',
                    400: '#34d399',
                    500: '#10b981',
                    600: '#059669',
                    700: '#047857',
                    800: '#065f46',
                    900: '#064e3b',
                  },
                  blue: {
                    50: '#eff6ff',
                    100: '#dbeafe',
                    200: '#bfdbfe',
                    300: '#93c5fd',
                    400: '#60a5fa',
                    500: '#3b82f6',
                    600: '#2563eb',
                    700: '#1d4ed8',
                    800: '#1e40af',
                    900: '#1e3a8a',
                  },
                  indigo: {
                    50: '#eef2ff',
                    100: '#e0e7ff',
                    200: '#c7d2fe',
                    300: '#a5b4fc',
                    400: '#818cf8',
                    500: '#6366f1',
                    600: '#4f46e5',
                    700: '#4338ca',
                    800: '#3730a3',
                    900: '#312e81',
                  },
                  purple: {
                    50: '#f5f3ff',
                    100: '#ede9fe',
                    200: '#ddd6fe',
                    300: '#c4b5fd',
                    400: '#a78bfa',
                    500: '#8b5cf6',
                    600: '#7c3aed',
                    700: '#6d28d9',
                    800: '#5b21b6',
                    900: '#4c1d95',
                  },
                  pink: {
                    50: '#fdf2f8',
                    100: '#fce7f3',
                    200: '#fbcfe8',
                    300: '#f9a8d4',
                    400: '#f472b6',
                    500: '#ec4899',
                    600: '#db2777',
                    700: '#be185d',
                    800: '#9d174d',
                    900: '#831843',
                  },

                  // Custom color schemes
                  base: {
                    DEFAULT: 'var(--color-base)',
                    50: 'var(--color-base-50)',
                    100: 'var(--color-base-100)',
                    200: 'var(--color-base-200)',
                    300: 'var(--color-base-300)',
                    400: 'var(--color-base-400)',
                    500: 'var(--color-base-500)',
                    600: 'var(--color-base-600)',
                    700: 'var(--color-base-700)',
                    800: 'var(--color-base-800)',
                    900: 'var(--color-base-900)',
                    content: 'var(--color-base-content)',
                  },
                  primary: {
                    DEFAULT: 'var(--color-primary)',
                    50: 'var(--color-primary-50)',
                    100: 'var(--color-primary-100)',
                    200: 'var(--color-primary-200)',
                    300: 'var(--color-primary-300)',
                    400: 'var(--color-primary-400)',
                    500: 'var(--color-primary-500)',
                    600: 'var(--color-primary-600)',
                    700: 'var(--color-primary-700)',
                    800: 'var(--color-primary-800)',
                    900: 'var(--color-primary-900)',
                    focus: 'var(--color-primary-focus)',
                    content: 'var(--color-primary-content)',
                  },
                  secondary: {
                    DEFAULT: 'var(--color-secondary)',
                    50: 'var(--color-secondary-50)',
                    100: 'var(--color-secondary-100)',
                    200: 'var(--color-secondary-200)',
                    300: 'var(--color-secondary-300)',
                    400: 'var(--color-secondary-400)',
                    500: 'var(--color-secondary-500)',
                    600: 'var(--color-secondary-600)',
                    700: 'var(--color-secondary-700)',
                    800: 'var(--color-secondary-800)',
                    900: 'var(--color-secondary-900)',
                    focus: 'var(--color-secondary-focus)',
                    content: 'var(--color-secondary-content)',
                  },
                  accent: {
                    DEFAULT: 'var(--color-accent)',
                    50: 'var(--color-accent-50)',
                    100: 'var(--color-accent-100)',
                    200: 'var(--color-accent-200)',
                    300: 'var(--color-accent-300)',
                    400: 'var(--color-accent-400)',
                    500: 'var(--color-accent-500)',
                    600: 'var(--color-accent-600)',
                    700: 'var(--color-accent-700)',
                    800: 'var(--color-accent-800)',
                    900: 'var(--color-accent-900)',
                    focus: 'var(--color-accent-focus)',
                    content: 'var(--color-accent-content)',
                  },
                  neutral: {
                    DEFAULT: 'var(--color-neutral)',
                    50: 'var(--color-neutral-50)',
                    100: 'var(--color-neutral-100)',
                    200: 'var(--color-neutral-200)',
                    300: 'var(--color-neutral-300)',
                    400: 'var(--color-neutral-400)',
                    500: 'var(--color-neutral-500)',
                    600: 'var(--color-neutral-600)',
                    700: 'var(--color-neutral-700)',
                    800: 'var(--color-neutral-800)',
                    900: 'var(--color-neutral-900)',
                    focus: 'var(--color-neutral-focus)',
                    content: 'var(--color-neutral-content)',
                  },
                  info: {
                    DEFAULT: 'var(--color-info)',
                    50: 'var(--color-info-50)',
                    100: 'var(--color-info-100)',
                    200: 'var(--color-info-200)',
                    300: 'var(--color-info-300)',
                    400: 'var(--color-info-400)',
                    500: 'var(--color-info-500)',
                    600: 'var(--color-info-600)',
                    700: 'var(--color-info-700)',
                    800: 'var(--color-info-800)',
                    900: 'var(--color-info-900)',
                    focus: 'var(--color-info-focus)',
                    content: 'var(--color-info-content)',
                  },
                  success: {
                    DEFAULT: 'var(--color-success)',
                    50: 'var(--color-success-50)',
                    100: 'var(--color-success-100)',
                    200: 'var(--color-success-200)',
                    300: 'var(--color-success-300)',
                    400: 'var(--color-success-400)',
                    500: 'var(--color-success-500)',
                    600: 'var(--color-success-600)',
                    700: 'var(--color-success-700)',
                    800: 'var(--color-success-800)',
                    900: 'var(--color-success-900)',
                    focus: 'var(--color-success-focus)',
                    content: 'var(--color-success-content)',
                  },
                  warning: {
                    DEFAULT: 'var(--color-warning)',
                    50: 'var(--color-warning-50)',
                    100: 'var(--color-warning-100)',
                    200: 'var(--color-warning-200)',
                    300: 'var(--color-warning-300)',
                    400: 'var(--color-warning-400)',
                    500: 'var(--color-warning-500)',
                    600: 'var(--color-warning-600)',
                    700: 'var(--color-warning-700)',
                    800: 'var(--color-warning-800)',
                    900: 'var(--color-warning-900)',
                    focus: 'var(--color-warning-focus)',
                    content: 'var(--color-warning-content)',
                  },
                  error: {
                    DEFAULT: 'var(--color-error)',
                    50: 'var(--color-error-50)',
                    100: 'var(--color-error-100)',
                    200: 'var(--color-error-200)',
                    300: 'var(--color-error-300)',
                    400: 'var(--color-error-400)',
                    500: 'var(--color-error-500)',
                    600: 'var(--color-error-600)',
                    700: 'var(--color-error-700)',
                    800: 'var(--color-error-800)',
                    900: 'var(--color-error-900)',
                    focus: 'var(--color-error-focus)',
                    content: 'var(--color-error-content)',
                  },
                  // Aliases
                  danger:  {
                    DEFAULT: 'var(--color-error)',
                    50: 'var(--color-error-50)',
                    100: 'var(--color-error-100)',
                    200: 'var(--color-error-200)',
                    300: 'var(--color-error-300)',
                    400: 'var(--color-error-400)',
                    500: 'var(--color-error-500)',
                    600: 'var(--color-error-600)',
                    700: 'var(--color-error-700)',
                    800: 'var(--color-error-800)',
                    900: 'var(--color-error-900)',
                    focus: 'var(--color-error-focus)',
                    content: 'var(--color-error-content)',
                  },
                  failure:  {
                    DEFAULT: 'var(--color-error)',
                    50: 'var(--color-error-50)',
                    100: 'var(--color-error-100)',
                    200: 'var(--color-error-200)',
                    300: 'var(--color-error-300)',
                    400: 'var(--color-error-400)',
                    500: 'var(--color-error-500)',
                    600: 'var(--color-error-600)',
                    700: 'var(--color-error-700)',
                    800: 'var(--color-error-800)',
                    900: 'var(--color-error-900)',
                    focus: 'var(--color-error-focus)',
                    content: 'var(--color-error-content)',
                  },
                },
              },
            },
            variants: {
              extend: {
                backgroundColor: ['active', 'group-hover'],
                textColor: ['active', 'group-hover'],
              },
            },
            plugins: [],
          };
      </script>
      </head>
              <body class="h-full text-base-content">
                <div id="root" class="bg-gray-50">
    <header id="header" class="bg-white shadow-sm">
        <nav class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="flex items-center">
                    <i class="fa-solid fa-brain text-purple-600 text-3xl mr-3"></i>
                    <span class="text-2xl font-bold text-purple-600">ActiveMind</span>
                </div>
                <div class="flex items-center space-x-6">
                    <span  class="text-lg text-gray-700 hover:text-purple-600 cursor-pointer">About</span>
                    <span  class="text-lg text-gray-700 hover:text-purple-600 cursor-pointer">Support</span>
                    <button class="bg-purple-600 text-white px-6 py-2 rounded-lg text-lg hover:bg-purple-700">Sign In</button>
                </div>
            </div>
        </nav>
    </header>
    <main>
        <section id="hero" class="h-[600px] bg-gradient-to-r from-purple-100 to-pink-50">
            <div class="container mx-auto px-6 py-20">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                    <div>
                        <h1 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">Stay Active, Stay Sharp with ActiveMind</h1>
                        <p class="text-xl text-gray-600 mb-8">Combine physical exercise with fun brain games designed specifically for active seniors.</p>
                        <button class="bg-purple-600 text-white text-xl px-8 py-4 rounded-lg hover:bg-purple-700">
                            <i class="fa-solid fa-play mr-2"></i>Start Your Journey
                        </button>
                    </div>
                    <div>
                        <img class="rounded-2xl shadow-xl" src="https://storage.googleapis.com/uxpilot-auth.appspot.com/e3709173ea-8206fc0da60c7ea6e7e5.png" alt="senior woman doing gentle exercise with a tablet, smiling, bright and cheerful setting, high quality photograph" >
                    </div>
                </div>
            </div>
        </section>
        <section id="features" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">Start Your Daily Exercise</h2>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition">
                        <div class="bg-purple-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                            <i class="fa-solid fa-dumbbell text-2xl text-purple-600"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-4">Physical Exercise</h3>
                        <p class="text-gray-600 text-lg mb-4">Gentle movements and stretches designed for your comfort and ability.</p>
                        <button class="text-purple-600 text-lg font-semibold hover:text-purple-700">
                            Start Exercise <i class="fa-solid fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition">
                        <div class="bg-purple-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                            <i class="fa-solid fa-puzzle-piece text-2xl text-purple-600"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-4">Brain Games</h3>
                        <p class="text-gray-600 text-lg mb-4">Fun puzzles and memory games to keep your mind active and engaged.</p>
                        <button class="text-purple-600 text-lg font-semibold hover:text-purple-700">
                            Play Games <i class="fa-solid fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition">
                        <div class="bg-purple-100 w-16 h-16 rounded-full flex items-center justify-center mb-6">
                            <i class="fa-solid fa-chart-line text-2xl text-purple-600"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-4">Track Progress</h3>
                        <p class="text-gray-600 text-lg mb-4">Monitor your achievements and see your improvement over time.</p>
                        <button class="text-purple-600 text-lg font-semibold hover:text-purple-700">
                            View Progress <i class="fa-solid fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                </div>
            </div>
        </section>
        <section id="testimonials" class="bg-purple-50 py-20">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl font-bold text-center text-gray-800 mb-12">What Our Members Say</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <div class="bg-white p-8 rounded-xl shadow-sm">
                        <div class="flex items-center mb-6">
                            <img src="https://storage.googleapis.com/uxpilot-auth.appspot.com/avatars/avatar-2.jpg" alt="Member" class="w-16 h-16 rounded-full mr-4"/>
                            <div>
                                <h4 class="text-xl font-bold text-gray-800">Margaret Wilson</h4>
                                <p class="text-gray-600">Active Member, 68</p>
                            </div>
                        </div>
                        <p class="text-gray-600 text-lg">"ActiveMind has made exercise fun again! I love how I can work on my physical fitness while playing engaging brain games."</p>
                    </div>
                    <div class="bg-white p-8 rounded-xl shadow-sm">
                        <div class="flex items-center mb-6">
                            <img src="https://storage.googleapis.com/uxpilot-auth.appspot.com/avatars/avatar-3.jpg" alt="Member" class="w-16 h-16 rounded-full mr-4"/>
                            <div>
                                <h4 class="text-xl font-bold text-gray-800">Patricia Thomas</h4>
                                <p class="text-gray-600">Active Member, 72</p>
                            </div>
                        </div>
                        <p class="text-gray-600 text-lg">"The exercises are perfect for my ability level, and I've noticed improvement in both my balance and memory."</p>
                    </div>
                </div>
            </div>
        </section>
        <section id="cta" class="py-20">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl font-bold text-gray-800 mb-6">Ready to Start Your Journey?</h2>
                <p class="text-xl text-gray-600 mb-8">Join thousands of active seniors who are improving their physical and mental wellness with ActiveMind.</p>
                <button class="bg-purple-600 text-white text-xl px-8 py-4 rounded-lg hover:bg-purple-700">
                    <i class="fa-solid fa-user-plus mr-2"></i>Join ActiveMind Today
                </button>
            </div>
        </section>
    </main>
    <footer id="footer" class="bg-gray-800 text-white py-12">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center mb-6">
                        <i class="fa-solid fa-brain text-purple-400 text-3xl mr-3"></i>
                        <span class="text-2xl font-bold text-white">ActiveMind</span>
                    </div>
                    <p class="text-gray-400">Empowering Seniors Through Movement</p>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><span  class="text-gray-400 hover:text-white cursor-pointer">About Us</span></li>
                        <li><span  class="text-gray-400 hover:text-white cursor-pointer">Exercise Programs</span></li>
                        <li><span  class="text-gray-400 hover:text-white cursor-pointer">Brain Games</span></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">Support</h4>
                    <ul class="space-y-2">
                        <li><span  class="text-gray-400 hover:text-white cursor-pointer">Help Center</span></li>
                        <li><span  class="text-gray-400 hover:text-white cursor-pointer">Contact Us</span></li>
                        <li><span  class="text-gray-400 hover:text-white cursor-pointer">Privacy Policy</span></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-lg font-bold mb-4">Connect With Us</h4>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white text-xl">
                            <i class="fa-brands fa-facebook"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white text-xl">
                            <i class="fa-brands fa-instagram"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white text-xl">
                            <i class="fa-brands fa-youtube"></i>
                        </a>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 text-center">
                <p class="text-gray-400">&copy; 2025 ActiveMind. All rights reserved.</p>
            </div>
        </div>
    </footer>
</div>
              </body>
            </html>
          
