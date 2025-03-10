- `CR ControlNet Input Switch`: This node serves as a dynamic switch between two control networks based on a specified input. It allows for the selection of one of two control networks to be used in a workflow, enhancing flexibility and control in the processing pipeline.
    - Inputs:
        - `Input` (Required): Determines which control network to select for use in the workflow. The choice affects the control flow and the resulting control network output. Type should be `INT`.
        - `control_net1` (Required): The first control network option that can be selected based on the input. Provides a pathway for control flow based on the selection. Type should be `CONTROL_NET`.
        - `control_net2` (Required): The second control network option that can be selected. Offers an alternative pathway for control flow, enhancing the node's flexibility. Type should be `CONTROL_NET`.
        - `control_net1` (Optional): The first control network option that can be selected based on the input. Provides a pathway for control flow based on the selection. Type should be `CONTROL_NET`.
        - `control_net2` (Optional): The second control network option that can be selected. Offers an alternative pathway for control flow, enhancing the node's flexibility. Type should be `CONTROL_NET`.
    - Outputs:
        - `CONTROL_NET`: The control network selected based on the input. This output is used for further processing in the workflow. Type should be `CONTROL_NET`.
        - `show_help`: A URL providing documentation and help for using the CR_ControlNetInputSwitch node. Type should be `STRING`.
