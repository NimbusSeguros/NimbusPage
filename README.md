
## Explicación de Carpetas

- **domain/**: Contiene toda la lógica de negocio independiente del framework
  - `models/`: Definiciones de tipos e interfaces
  - `ports/`: Contratos/interfaces para implementaciones externas
  - `use-cases/`: Casos de uso principales de la aplicación

- **infrastructure/**: Implementaciones concretas de los puertos definidos
  - `services/`: Conexiones con APIs externas
  - `storage/`: Manejo de almacenamiento local

- **application/**: Capa que adapta el dominio a la UI
  - `contexts/`: Estado global de React
  - `hooks/`: Custom hooks reutilizables
  - `utils/`: Funciones de transformación de datos

- **presentation/**: Componentes de UI
  - `components/ui/`: Componentes presentacionales (sin estado)
  - `components/features/`: Componentes con lógica específica
  - `pages/`: Componentes de páginas/rutas
  - `assets/`: Recursos estáticos

- **shared/**: Utilidades compartidas
  - `constants/`: Constantes de la aplicación
  - `styles/`: Configuración de estilos globales

- **App.tsx**: Componente raíz de la aplicación
