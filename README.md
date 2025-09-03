# Prompts

These are copied from https://github.com/VoloBuilds/prompts

And I'm planning to add some of my own

plan_feature.md

Prompt:
Use the plan_feature.md file to create a new plan file. Add the following to the plan: <add prompt here>

--------------

code_review.md

Prompt:
Use the code_review.md file to create a new review file based on the following plan docs/features/0006_PLAN.md 

--------------

create_brief.md

Prompt:
Use the create_brief.md file to create a new brief file based on this project.

--------------

write_docs.md

---------------

### Project Feature Audit Command

#### Usage (in Cursor IDE)

##### Option 1
```
@list_project_features.md 
Please audit my React project using this template
```

##### Option 2
```
@list_project_features.md 
audit-project [REPO_PATH] [OPTIONS]
```

##### Option 3
```
@list_project_features.md 
audit-project . --output="./PROJECT_FEATURES.md"
```

--------------

we need a plan.md file for refactoring

we need a plan.md file for creating a project brief for an existing project

we need a plan.md file for explaining the structure of a backend or frontend project
