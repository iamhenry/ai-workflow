# Generating Task List  

# Principles
- Always think step by step

# Instructions
Create a detailed task plan for developing a software feature, ensuring the following structure:  

1. Divide the feature into milestones
    Each milestone should represent a significant deliverable or phase of the project. Include a clear objective describing the goal of the milestone and acceptance criteria defining what qualifies the milestone as complete.  
2. Break down each milestone into tasks
    Each task should be tightly scoped, actionable, small, and independent. Use clear language for what the task involves.  
3. Specify dependencies
    Identify and document relationships between tasks, indicating which tasks depend on others.
4. Include file references
    For each task, specify which file(s) to modify, and note if a file needs to be created.
5. Format the tasks as markdown checkboxes
    Use markdown formatting to ensure tasks are easy to track and check off.

<output_format>
Use the following example structure:   

```markdown
# [Task Plan Name]

## Milestone [Number]: [Milestone Title]

## Relevant Files:
[List relevant primary and secondary files. Include purpose of that file in a inline comment]

# Data Flow:
[Outline the flow of data between frontend and backend, detailing what is sent (e.g., form data, API requests), how it is processed on the server (e.g., validation, database interactions), and what is returned to the frontend (e.g., responses, data rendering). Include key interactions between components, API routes, and database queries.]

## Objective:
[Describe the specific goal of the milestone.]

## Acceptance Criteria:
- [List the measurable outcomes that define milestone success.]

## Step-by-Step Tasks:
- [ ] [Task Number]. [Task Description]
  - File: `[File Name]` ([specify if it needs to be created]).
  - Dependency: [Specify dependency if applicable].
```
</output_format>

<commands>
/status = mark completed tasks as done and list next steps
</commands>

[No code blocks in the final task list]