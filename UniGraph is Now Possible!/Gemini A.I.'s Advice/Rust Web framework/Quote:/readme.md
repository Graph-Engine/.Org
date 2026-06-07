# Recommended Stack Recommendation
Given your vision of thousands of distinct, highly customized communities running off a massive graph backend, a dual-layer approach will scale cleanly:

1. The Backend API Layer: Use Axum. Its modular architecture allows you to easily isolate your graph query routing logic. This is also where you can safely mount your custom WebAssembly sandbox engine for contributor code.
2. The Frontend UI Layer: Use Leptos. It offers maximum performance for web deployment, keeps your UI entirely in Rust, handles SEO beautifully via SSR, and streamlines browser-to-server data transmission.
