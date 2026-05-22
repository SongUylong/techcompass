# Architecture Notes

## Apps

- `frontend`: Next.js user dashboard
- `backend`: Laravel API

## Data Flow

1. User selects career domain and skill baseline.
2. Backend stores profile and retrieves curated resources.
3. Neuron AI RAG uses cleaned data to generate a learning path.
4. Frontend shows roadmap, milestones, projects, and progress.

