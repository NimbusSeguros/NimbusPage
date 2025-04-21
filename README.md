src/
│
├── domain/                # Lógica de negocio (independiente de React)
│   ├── models/            # Entidades/Tipos (ej: `User.ts`, `Policy.ts`)
│   ├── ports/             # Interfaces/contratos (ej: `AuthRepository.ts`)
│   └── use-cases/         # Lógica de aplicación (ej: `LoginUseCase.ts`)
│
├── infrastructure/        # Implementaciones concretas
│   ├── services/          # Conexiones a APIs (ej: `AuthService.ts`)
│   └── storage/           # Manejo de localStorage/sessionStorage
│
├── application/           # Adaptadores para la UI
│   ├── contexts/          # Contextos de React (ej: `AuthContext.tsx`)
│   ├── hooks/             # Custom hooks (ej: `useAuth.ts`)
│   └── utils/             # Adaptadores de datos (ej: `policyMapper.ts`)
│
├── presentation/          # Capa de UI (React)
│   ├── components/        # Componentes reutilizables
│   │   ├── ui/            # Componentes "tontos" (ej: `Button.tsx`)
│   │   └── features/      # Componentes con lógica (ej: `PolicyCard.tsx`)
│   ├── pages/             # Páginas/rutas (ej: `LoginPage.tsx`)
│   └── assets/            # Imágenes, estilos globales
│
├── shared/                # Utilidades comunes
│   ├── constants/         # (ej: `routes.ts`)
│   └── styles/            # Config de Tailwind/global CSS
│
└── App.tsx                # Entrada principal
