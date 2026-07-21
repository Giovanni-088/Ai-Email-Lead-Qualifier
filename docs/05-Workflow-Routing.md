# Workflow Routing

## Objective

Route each lead according to the AI classification.

## Workflow

```text
Google Sheets Trigger
        │
        ▼
Groq (Llama 3.3)
        │
        ▼
JSON Parser
        │
        ▼
IF
├── HOT
├── WARM
└── COLD
```

## Conditions

### HOT

```
classification == HOT
```

### WARM

```
classification == WARM
```

### COLD

```
classification == COLD
```

## Output

Every lead is routed to its corresponding automation path.

The next phases will implement the actions executed for each branch.
