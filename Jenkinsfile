{
    "author": "artemry@mellanox.com",
    "notify": "artemry@mellanox.com",
    "ci_version": "1.0",
    "parameters": {"PARAM1": "VALUE1", "PARAM2": "VALUE2"},
    "timeout": 180,
    "phases":
        [
            {
                "phase_1":
                [
                    {
                        "name": "Clone",
                        "module": "ci_framework/modules/generic_modules/checkout.groovy",
                        "category": "Clone",
                        "node": "hpc-test-node-gpu",
                        "parameters": {"BRANCH_NAME": "master","GIT_REPOSITORY": "git@gitlab.com:Mellanox/ml-devops-infra.git", "CLONE_PATH": "ml-devops-infra"},
                        "skip": false,
                        "ignore_failure": false,
                        "finally": false
                    },
                    {
                        "name": "Spell Check",
                        "module": "ci_framework/modules/generic_modules/spell_check.groovy",
                        "category": "Pre Build",
                        "node": "hpc-test-node-gpu",
                        "parameters": {},
                        "skip": false,
                        "ignore_failure": false,
                        "finally": false
                    }
                ]
            }
        ]
}
