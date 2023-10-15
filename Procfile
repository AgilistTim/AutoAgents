# Creating the content for Procfile and setup.sh

procfile_content = "web: streamlit run autoagents/agents/spaces/app.py"
setup_sh_content = """
mkdir -p ~/.streamlit/
echo "\
[server]\\n\
headless = true\\n\
port = $PORT\\n\
enableCORS = false\\n\
\\n\
" > ~/.streamlit/config.toml
"""

# Saving the content to files
procfile_path = os.path.join(extract_path, 'AutoAgents', 'Procfile')
setup_sh_path = os.path.join(extract_path, 'AutoAgents', 'setup.sh')

with open(procfile_path, 'w') as f:
    f.write(procfile_content)

with open(setup_sh_path, 'w') as f:
    f.write(setup_sh_content)

procfile_path, setup_sh_path
