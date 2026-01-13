# @zylos/shared-types

Shared TypeScript types and Zod schemas for Zylos ERP/POS system.

## Installation

```bash
npm install @zylos/shared-types
```

## Usage

```typescript
import { Database, User, Tenant, UserRole } from '@zylos/shared-types'

// Use the Database type for Supabase client
type SupabaseClient = SupabaseClient<Database>

// Use entity types
const user: User = {
  id: '123',
  email: 'user@example.com',
  tenant_id: '456',
  role: 'admin',
  created_at: new Date().toISOString(),
  updated_at: new Date().toISOString()
}
```

## Published Types

- **Database**: Complete Supabase database schema
- **Entities**: User, Tenant, Product, Customer, Supplier, etc.
- **API Responses**: AuthResponse, ApiResponse
- **Common Enums**: UserRole, EntityType, MovementType, etc.

## Development

```bash
npm run dev    # Watch mode
npm run build  # Build for publishing
```

## License

MIT