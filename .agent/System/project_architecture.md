# Project Architecture

**Last Updated:** 2025-10-06

## Related Documentation
- [.agent/README.md](../README.md) - Documentation index

---

## 🎯 Project Goal

The electromagnetic-simulation-agent is an open-source project designed to expedite electromagnetic simulation workflows by utilizing an AI agent that can interact with CST Studio Suite to create, edit, and refine component designs.

### Key Objectives
- Automate electromagnetic simulation design processes
- Enable natural language interaction with CST Studio Suite
- Accelerate iteration cycles for component design
- Reduce manual effort in simulation setup and refinement

---

## 🏗️ Project Structure

```
electromagnetic-simulation-agent/
├── README.md                    # Project overview
├── .agent/                      # Documentation directory
│   ├── README.md               # Documentation index
│   ├── System/                 # System documentation
│   │   └── project_architecture.md
│   ├── Tasks/                  # Feature PRDs and plans
│   └── SOP/                    # Standard operating procedures
└── my-app/                     # Application directory (to be developed)
    └── .claude/                # Claude AI configuration
        ├── CLAUDE.md           # Claude documentation guidelines
        └── Commands/
            └── update-doc.md   # Documentation update command
```

---

## 🛠️ Tech Stack

### Current State
The project is in its initial phase with the following components:

**Documentation & Planning:**
- Markdown-based documentation system
- Claude AI integration for documentation management

### Planned Stack (To Be Determined)
The following components will be needed as the project develops:

**AI/Agent Framework:**
- LLM integration (e.g., OpenAI, Anthropic Claude)
- Agent orchestration framework (e.g., LangChain, AutoGen)

**CST Studio Suite Integration:**
- CST API/scripting interface
- VBA or Python scripting for CST automation

**Backend:**
- Python (likely choice for CST integration and AI orchestration)
- API framework (FastAPI, Flask, or similar)

**Frontend (if applicable):**
- Web interface for agent interaction
- Visualization of simulation results

---

## 🔌 Integration Points

### CST Studio Suite
- **Purpose:** Primary electromagnetic simulation software
- **Integration Method:** To be determined (likely VBA scripting or Python API)
- **Capabilities Needed:**
  - Create and modify simulation models
  - Run simulations
  - Extract and analyze results
  - Parameter sweeps and optimization

### AI/LLM Integration
- **Purpose:** Natural language understanding and agent decision-making
- **Integration Method:** API calls to LLM providers
- **Capabilities Needed:**
  - Parse user intent from natural language
  - Generate CST commands/scripts
  - Interpret simulation results
  - Suggest design refinements

---

## 🤖 Agent Architecture

### Planned Components

**1. Natural Language Interface**
- Accepts user requests in natural language
- Translates intent into actionable simulation tasks

**2. Task Planning & Orchestration**
- Breaks down complex requests into subtasks
- Manages workflow execution
- Handles error recovery and retries

**3. CST Interface Layer**
- Translates high-level commands to CST-specific operations
- Manages CST Studio Suite connection
- Executes simulation commands

**4. Result Analysis & Feedback**
- Analyzes simulation outputs
- Provides insights and recommendations
- Suggests design improvements

**5. Memory & Context Management**
- Maintains conversation history
- Tracks design iterations
- Stores simulation parameters and results

---

## 🗄️ Database Schema

**Status:** Not yet implemented

As the project develops, a database will be needed to store:
- User sessions and conversation history
- Simulation configurations and parameters
- Design iterations and versions
- Simulation results and metadata
- Agent learning data and preferences

---

## 🚀 Development Status

### Phase 1: Foundation (Current)
- ✅ Project initialization
- ✅ Documentation structure established
- ⏳ Technology stack selection
- ⏳ Architecture design

### Phase 2: Core Development (Planned)
- ⏳ CST Studio Suite integration
- ⏳ AI agent implementation
- ⏳ Basic command execution
- ⏳ Result parsing and feedback

### Phase 3: Enhancement (Future)
- ⏳ Advanced agent capabilities
- ⏳ Multi-step workflows
- ⏳ Optimization algorithms
- ⏳ User interface development

---

## 📋 Next Steps

1. **Define detailed requirements** for CST integration
2. **Select and set up** AI/agent framework
3. **Prototype** basic CST command execution
4. **Implement** core agent loop
5. **Test** with simple simulation scenarios
6. **Iterate** based on results and feedback

---

## 🤝 Contributing

As this is an open-source project, contributions are welcome. Please ensure:
- All code changes are documented
- System documentation is updated to reflect architectural changes
- New features include corresponding documentation in .agent/Tasks/
- Standard procedures are documented in .agent/SOP/

---

## 📚 Additional Resources

- [CST Studio Suite Documentation](https://www.3ds.com/products-services/simulia/products/cst-studio-suite/)
- Project-specific resources to be added as development progresses
