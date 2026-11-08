![Hyperstream Client](./hyperstream-client.png)

# Hyperstream Client

Hyperstream Client is the web application for Access Layer, a creator-key marketplace connecting creators with their communities. It brings discovery, creator profiles, key trading, wallet activity, and creator and protocol tools into one interface.

## Product areas

- Discover creators, keys, bundles, campaigns, and community activity.
- View creator profiles, dashboards, revenue, and audience leaderboards.
- Manage wallet portfolios, trades, staking, governance, and transaction history.
- Connect wallets and work with the network and API settings documented in the environment guide.

## Technology

React 19, TypeScript, Vite, Tailwind CSS, React Router, TanStack Query, and Vitest.

## Development

Requirements: Node.js 20+ and pnpm 10.6.5.

```bash
pnpm install
cp .env.example .env
pnpm dev
```

Environment variables and network configuration are documented in [docs/environment-variables.md](./docs/environment-variables.md). The defaults support local frontend development; connecting to live services may require additional configuration.

## Verification

Run the same checks used by CI:

```bash
pnpm lint
pnpm build
```

Run the frontend test suite with `pnpm test`.

## Contributing

- Read [CONTRIBUTING.md](./CONTRIBUTING.md) for setup and pull request guidance.
- Check [the contributor backlog](./docs/open-source/issue-backlog.md) for potential work areas, then confirm an item is still relevant before starting.
- Use the issue templates in [`.github/ISSUE_TEMPLATE`](./.github/ISSUE_TEMPLATE).
- Review [SECURITY.md](./SECURITY.md) before reporting vulnerabilities.

## Keyboard shortcuts

- `Ctrl/Cmd + Alt + R` refreshes creator list data from the marketplace page. The shortcut is ignored while focus is inside text inputs, textareas, selects, or editable text regions.
- `T` opens the trade panel from the creator profile page. The shortcut is ignored while focus is inside text inputs, textareas, selects, or editable text regions.
