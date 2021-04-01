# OPTIC Plan solver

This package contains a plan solver that uses [OPTIC] for solving PDDL plans.

# Requirements

install optic: https://nms.kcl.ac.uk/planning/software/optic.html

This plugin is made for Plansys2 (https://github.com/IntelligentRoboticsLabs/ros2_planning_system), you must installed both plansys2 to try this plugin

To add plansys2 optic plugin to plansys2, clone the repository into ros2_planning_system folder.

modify /ros2_planning_system/plansys2_bringup/params/plansys2_params.yaml to add OPTIC

```
planner:
  ros__parameters:
    plan_solver_plugins: ["OPTIC"]
    POPF:
      plugin: "plansys2/POPFPlanSolver"
    TFD:
      plugin: "plansys2::TFDPlanSolver"
    OPTIC:
      plugin: "plansys2/OPTICPlanSolver"
```
