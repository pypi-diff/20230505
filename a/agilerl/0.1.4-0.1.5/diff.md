# Comparing `tmp/agilerl-0.1.4.tar.gz` & `tmp/agilerl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agilerl-0.1.4.tar", max compression
+gzip compressed data, was "agilerl-0.1.5.tar", max compression
```

## Comparing `agilerl-0.1.4.tar` & `agilerl-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,47 @@
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.4/agilerl/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.4/agilerl/algorithms/__init__.py
--rw-r--r--   0        0        0    16027 2023-04-04 16:17:27.795084 agilerl-0.1.4/agilerl/algorithms/ddpg.py
--rw-r--r--   0        0        0    11492 2023-04-04 16:17:27.795084 agilerl-0.1.4/agilerl/algorithms/dqn.py
--rw-r--r--   0        0        0     4950 2023-04-04 16:17:27.796081 agilerl-0.1.4/agilerl/benchmarking.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.238404 agilerl-0.1.4/agilerl/components/__init__.py
--rw-r--r--   0        0        0     3783 2023-04-04 16:17:27.797079 agilerl-0.1.4/agilerl/components/replay_buffer.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.239407 agilerl-0.1.4/agilerl/hpo/__init__.py
--rw-r--r--   0        0        0    16930 2023-04-04 16:17:27.798076 agilerl-0.1.4/agilerl/hpo/mutation.py
--rw-r--r--   0        0        0     2121 2023-03-09 14:51:00.360677 agilerl-0.1.4/agilerl/hpo/tournament.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.241395 agilerl-0.1.4/agilerl/networks/__init__.py
--rw-r--r--   0        0        0    24254 2023-04-04 16:17:27.799075 agilerl-0.1.4/agilerl/networks/evolvable_cnn.py
--rw-r--r--   0        0        0    14965 2023-04-04 16:17:27.799075 agilerl-0.1.4/agilerl/networks/evolvable_mlp.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.242405 agilerl-0.1.4/agilerl/training/__init__.py
--rw-r--r--   0        0        0     6801 2023-04-04 16:17:27.800071 agilerl-0.1.4/agilerl/training/train.py
--rw-r--r--   0        0        0     3389 2023-04-04 16:17:27.801069 agilerl-0.1.4/agilerl/utils.py
--rw-r--r--   0        0        0    11558 2023-03-06 12:15:09.243395 agilerl-0.1.4/LICENSE
--rw-r--r--   0        0        0      550 2023-04-04 16:18:04.209485 agilerl-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    16274 2023-04-04 16:17:27.794086 agilerl-0.1.4/README.md
--rw-r--r--   0        0        0    16880 1970-01-01 00:00:00.000000 agilerl-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.5/agilerl/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.5/agilerl/algorithms/__init__.py
+-rw-r--r--   0        0        0    20456 2023-05-05 09:35:55.662695 agilerl-0.1.5/agilerl/algorithms/bc_lm.py
+-rw-r--r--   0        0        0    17131 2023-05-05 09:35:55.670696 agilerl-0.1.5/agilerl/algorithms/ddpg.py
+-rw-r--r--   0        0        0    12025 2023-05-05 09:35:55.670696 agilerl-0.1.5/agilerl/algorithms/dqn.py
+-rw-r--r--   0        0        0    72764 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/algorithms/ilql.py
+-rw-r--r--   0        0        0     5486 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/benchmarking.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.238404 agilerl-0.1.5/agilerl/components/__init__.py
+-rw-r--r--   0        0        0     3874 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/components/replay_buffer.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/data/__init__.py
+-rw-r--r--   0        0        0     1688 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/language_environment.py
+-rw-r--r--   0        0        0     8013 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/rl_data.py
+-rw-r--r--   0        0        0     1303 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/tokenizer.py
+-rw-r--r--   0        0        0     1175 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/torch_datasets.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.239407 agilerl-0.1.5/agilerl/hpo/__init__.py
+-rw-r--r--   0        0        0    19911 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/hpo/mutation.py
+-rw-r--r--   0        0        0     2153 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/hpo/tournament.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.241395 agilerl-0.1.5/agilerl/networks/__init__.py
+-rw-r--r--   0        0        0    37557 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/networks/evolvable_bert.py
+-rw-r--r--   0        0        0    25101 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/networks/evolvable_cnn.py
+-rw-r--r--   0        0        0    37684 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/networks/evolvable_gpt.py
+-rw-r--r--   0        0        0    14781 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/networks/evolvable_mlp.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.242405 agilerl-0.1.5/agilerl/training/__init__.py
+-rw-r--r--   0        0        0     7408 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/training/train.py
+-rw-r--r--   0        0        0     8771 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/training/train_bc_lm.py
+-rw-r--r--   0        0        0     9326 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/training/train_ilql.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/utils/__init__.py
+-rw-r--r--   0        0        0     1628 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/utils/cache.py
+-rw-r--r--   0        0        0     3952 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/ilql_utils.py
+-rw-r--r--   0        0        0    10349 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/load_objects.py
+-rw-r--r--   0        0        0     2444 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/log_utils.py
+-rw-r--r--   0        0        0      120 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/mp_cache.py
+-rw-r--r--   0        0        0     2205 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/sampling_utils.py
+-rw-r--r--   0        0        0     3307 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/utils/serve_queue.py
+-rw-r--r--   0        0        0     1496 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/utils/torch_utils.py
+-rw-r--r--   0        0        0     3389 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/wordle/__init__.py
+-rw-r--r--   0        0        0     7021 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/wordle/policy.py
+-rw-r--r--   0        0        0     5900 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_dataset.py
+-rw-r--r--   0        0        0     1119 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_env.py
+-rw-r--r--   0        0        0     9110 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_evaluators.py
+-rw-r--r--   0        0        0    11117 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_game.py
+-rw-r--r--   0        0        0     2510 2023-05-05 09:35:55.736340 agilerl-0.1.5/agilerl/wordle/wordle_tokenizer.py
+-rw-r--r--   0        0        0    11558 2023-03-06 12:15:09.243395 agilerl-0.1.5/LICENSE
+-rw-r--r--   0        0        0      550 2023-05-05 09:36:45.006777 agilerl-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    18536 2023-05-05 09:35:55.662695 agilerl-0.1.5/README.md
+-rw-r--r--   0        0        0    19107 1970-01-01 00:00:00.000000 agilerl-0.1.5/PKG-INFO
```

### Comparing `agilerl-0.1.4/agilerl/algorithms/ddpg.py` & `agilerl-0.1.5/agilerl/algorithms/ddpg.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from agilerl.networks.evolvable_mlp import EvolvableMLP
 from agilerl.networks.evolvable_cnn import EvolvableCNN
 
+
 class DDPG():
     """The DDPG algorithm class. DDPG paper: https://arxiv.org/abs/1509.02971
 
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
@@ -33,16 +34,34 @@
     :param mutation: Most recent mutation to agent, defaults to None
     :type mutation: str, optional
     :param policy_freq: Frequency of target network updates compared to policy network, defaults to 2
     :type policy_freq: int, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
-    def __init__(self, state_dim, action_dim, one_hot, index=0, net_config={'arch':'mlp','h_size':[64,64]}, batch_size=64, 
-                 lr=1e-4, learn_step=5, gamma=0.99, tau=1e-3, mutation=None, policy_freq=2, device='cpu'):
+
+    def __init__(
+        self,
+        state_dim,
+        action_dim,
+        one_hot,
+        index=0,
+        net_config={
+            'arch': 'mlp',
+            'h_size': [
+            64,
+            64]},
+            batch_size=64,
+            lr=1e-4,
+            learn_step=5,
+            gamma=0.99,
+            tau=1e-3,
+            mutation=None,
+            policy_freq=2,
+            device='cpu'):
         self.algo = 'DDPG'
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.one_hot = one_hot
         self.net_config = net_config
         self.batch_size = batch_size
         self.lr = lr
@@ -56,64 +75,123 @@
         self.index = index
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
         # model
         if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
-            self.actor = EvolvableMLP(num_inputs=state_dim[0], num_outputs=action_dim, hidden_size=self.net_config['h_size'], output_activation='tanh', device=self.device).to(self.device)
-            self.actor_target = EvolvableMLP(num_inputs=state_dim[0], num_outputs=action_dim, hidden_size=self.net_config['h_size'], output_activation='tanh', device=self.device).to(self.device)
+            self.actor = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config['h_size'],
+                output_activation='tanh',
+                device=self.device).to(
+                self.device)
+            self.actor_target = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config['h_size'],
+                output_activation='tanh',
+                device=self.device).to(
+                self.device)
             self.actor_target.load_state_dict(self.actor.state_dict())
-            
-            self.critic = EvolvableMLP(num_inputs=state_dim[0]+action_dim, num_outputs=1, hidden_size=self.net_config['h_size'], device=self.device).to(self.device)
-            self.critic_target = EvolvableMLP(num_inputs=state_dim[0]+action_dim, num_outputs=1, hidden_size=self.net_config['h_size'], device=self.device).to(self.device)
+
+            self.critic = EvolvableMLP(
+                num_inputs=state_dim[0] + action_dim,
+                num_outputs=1,
+                hidden_size=self.net_config['h_size'],
+                device=self.device).to(
+                self.device)
+            self.critic_target = EvolvableMLP(
+                num_inputs=state_dim[0] + action_dim,
+                num_outputs=1,
+                hidden_size=self.net_config['h_size'],
+                device=self.device).to(
+                self.device)
             self.critic_target.load_state_dict(self.critic.state_dict())
 
         elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
-            self.actor = EvolvableCNN(input_shape=state_dim, num_actions=action_dim, channel_size=self.net_config['c_size'], kernal_size=self.net_config['k_size'],
-                                      stride_size=self.net_config['s_size'], hidden_size=self.net_config['h_size'], mlp_activation='tanh', device=self.device).to(self.device)
-            self.actor_target = EvolvableCNN(input_shape=state_dim, num_actions=action_dim, channel_size=self.net_config['c_size'], kernal_size=self.net_config['k_size'],
-                                             stride_size=self.net_config['s_size'], hidden_size=self.net_config['h_size'], mlp_activation='tanh', device=self.device).to(self.device)
+            self.actor = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config['c_size'],
+                kernal_size=self.net_config['k_size'],
+                stride_size=self.net_config['s_size'],
+                hidden_size=self.net_config['h_size'],
+                mlp_activation='tanh',
+                device=self.device).to(
+                self.device)
+            self.actor_target = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config['c_size'],
+                kernal_size=self.net_config['k_size'],
+                stride_size=self.net_config['s_size'],
+                hidden_size=self.net_config['h_size'],
+                mlp_activation='tanh',
+                device=self.device).to(
+                self.device)
             self.actor_target.load_state_dict(self.actor.state_dict())
-            
-            self.critic = EvolvableCNN(input_shape=state_dim, num_actions=action_dim, channel_size=self.net_config['c_size'], kernal_size=self.net_config['k_size'],
-                                      stride_size=self.net_config['s_size'], hidden_size=self.net_config['h_size'], mlp_activation='tanh', critic=True, device=self.device).to(self.device)
-            self.critic_target = EvolvableCNN(input_shape=state_dim, num_actions=action_dim, channel_size=self.net_config['c_size'], kernal_size=self.net_config['k_size'],
-                                             stride_size=self.net_config['s_size'], hidden_size=self.net_config['h_size'], mlp_activation='tanh', critic=True, device=self.device).to(self.device)
+
+            self.critic = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config['c_size'],
+                kernal_size=self.net_config['k_size'],
+                stride_size=self.net_config['s_size'],
+                hidden_size=self.net_config['h_size'],
+                mlp_activation='tanh',
+                critic=True,
+                device=self.device).to(
+                self.device)
+            self.critic_target = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config['c_size'],
+                kernal_size=self.net_config['k_size'],
+                stride_size=self.net_config['s_size'],
+                hidden_size=self.net_config['h_size'],
+                mlp_activation='tanh',
+                critic=True,
+                device=self.device).to(
+                self.device)
             self.critic_target.load_state_dict(self.critic.state_dict())
 
         self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
-        self.critic_optimizer = optim.Adam(self.critic.parameters(), lr=self.lr)
+        self.critic_optimizer = optim.Adam(
+            self.critic.parameters(), lr=self.lr)
         self.criterion = nn.MSELoss()
 
     def getAction(self, state, epsilon=0):
         """Returns the next action to take in the environment. Epsilon is the probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: Environment observation, or multiple observations in a batch
         :type state: float or List[float]
         :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
         :type epsilon: float, optional
         """
         state = torch.from_numpy(state).float().to(self.device)
 
         if self.one_hot:
-            state = nn.functional.one_hot(state.long(), num_classes=self.state_dim[0]).float().squeeze()
-        
-        if len(state.size())<2:
+            state = nn.functional.one_hot(
+                state.long(), num_classes=self.state_dim[0]).float().squeeze()
+
+        if len(state.size()) < 2:
             state = state.unsqueeze(0)
 
         self.actor.eval()
         with torch.no_grad():
             action_values = self.actor(state)
         self.actor.train()
 
         # epsilon-greedy
         if random.random() < epsilon:
-            action = (np.random.rand(state.size()[0], self.action_dim).astype('float32')-0.5)*2
+            action = (np.random.rand(
+                state.size()[0], self.action_dim).astype('float32') - 0.5) * 2
         else:
             action = action_values.cpu().data.numpy()
 
         return action
 
     def learn(self, experiences, noise_clip=0.5, policy_noise=0.2):
         """Updates agent network parameters to learn from experiences.
@@ -124,16 +202,18 @@
         :type noise_clip: float, optional
         :param policy_noise: Standard deviation of noise applied to policy, defaults to 0.2
         :type policy_noise: float, optional
         """
         states, actions, rewards, next_states, dones = experiences
 
         if self.one_hot:
-            states = nn.functional.one_hot(states.long(), num_classes=self.state_dim[0]).float().squeeze()
-            next_states = nn.functional.one_hot(next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
+            states = nn.functional.one_hot(
+                states.long(), num_classes=self.state_dim[0]).float().squeeze()
+            next_states = nn.functional.one_hot(
+                next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
 
         if self.net_config['arch'] == 'mlp':
             input_combined = torch.cat([states, actions], 1)
             q_value = self.critic(input_combined)
         elif self.net_config['arch'] == 'cnn':
             q_value = self.critic(states, actions)
 
@@ -143,45 +223,48 @@
         next_actions = (next_actions + noise)
 
         if self.net_config['arch'] == 'mlp':
             next_input_combined = torch.cat([next_states, next_actions], 1)
             q_value_next_state = self.critic_target(next_input_combined)
         elif self.net_config['arch'] == 'cnn':
             q_value_next_state = self.critic(next_states, next_actions)
-        
+
         y_j = rewards + (self.gamma * q_value_next_state).detach()
 
         critic_loss = self.criterion(q_value, y_j)
 
         # critic loss backprop
         self.critic_optimizer.zero_grad()
         critic_loss.backward()
         self.critic_optimizer.step()
 
         # update actor and targets every policy_freq episodes
         if len(self.scores) % self.policy_freq == 0:
             if self.net_config['arch'] == 'mlp':
-                input_combined = torch.cat([states, self.actor.forward(states)], 1)
+                input_combined = torch.cat(
+                    [states, self.actor.forward(states)], 1)
                 actor_loss = -self.critic(input_combined).mean()
             elif self.net_config['arch'] == 'cnn':
-                actor_loss = -self.critic(states, self.actor.forward(states)).mean()
-            
+                actor_loss = - \
+                    self.critic(states, self.actor.forward(states)).mean()
+
             # actor loss backprop
             self.actor_optimizer.zero_grad()
             actor_loss.backward()
             self.actor_optimizer.step()
 
             self.softUpdate(self.actor, self.actor_target)
             self.softUpdate(self.critic, self.critic_target)
 
     def softUpdate(self, net, target):
         """Soft updates target network.
         """
         for eval_param, target_param in zip(net.parameters(), target.parameters()):
-            target_param.data.copy_(self.tau*eval_param.data + (1.0-self.tau)*target_param.data)
+            target_param.data.copy_(
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
         :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
@@ -213,99 +296,109 @@
         :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
         clone = type(self)(state_dim=self.state_dim,
-                            action_dim=self.action_dim,
-                            one_hot=self.one_hot,
-                            index=index, 
-                            net_config = self.net_config, 
-                            batch_size=self.batch_size,
-                            lr=self.lr,
-                            learn_step=self.learn_step,
-                            gamma=self.gamma,
-                            tau=self.tau,
-                            mutation=self.mut,
-                            policy_freq=self.policy_freq,
-                            device=self.device,
+                           action_dim=self.action_dim,
+                           one_hot=self.one_hot,
+                           index=index,
+                           net_config=self.net_config,
+                           batch_size=self.batch_size,
+                           lr=self.lr,
+                           learn_step=self.learn_step,
+                           gamma=self.gamma,
+                           tau=self.tau,
+                           mutation=self.mut,
+                           policy_freq=self.policy_freq,
+                           device=self.device,
                            )
-                           
+
         clone.actor = self.actor.clone().to(self.device)
         clone.actor_target = self.actor_target.clone().to(self.device)
         clone.critic = self.critic.clone().to(self.device)
         clone.critic_target = self.critic_target.clone().to(self.device)
 
-        clone.actor_optimizer = optim.Adam(clone.actor.parameters(), lr=clone.lr)
-        clone.critic_optimizer = optim.Adam(clone.critic.parameters(), lr=clone.lr)
+        clone.actor_optimizer = optim.Adam(
+            clone.actor.parameters(), lr=clone.lr)
+        clone.critic_optimizer = optim.Adam(
+            clone.critic.parameters(), lr=clone.lr)
 
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
-    
+
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
         torch.save({
-                    'actor_init_dict': self.actor.init_dict,
-                    'actor_state_dict': self.actor.state_dict(),
-                    'actor_target_init_dict': self.actor_target.init_dict,
-                    'actor_target_state_dict': self.actor_target.state_dict(),
-                    'critic_init_dict': self.critic.init_dict,
-                    'critic_state_dict': self.critic.state_dict(),
-                    'critic_target_init_dict': self.critic_target.init_dict,
-                    'critic_target_state_dict': self.critic_target.state_dict(),
-                    'actor_optimizer_state_dict': self.actor_optimizer.state_dict(),
-                    'critic_optimizer_state_dict': self.critic_optimizer.state_dict(),
-                    'net_config': self.net_config,
-                    'batch_size': self.batch_size,
-                    'lr': self.lr,
-                    'learn_step': self.learn_step,
-                    'gamma': self.gamma,
-                    'tau': self.tau,
-                    'mutation': self.mut,
-                    'index': self.index, 
-                    'scores': self.scores,
-                    'fitness': self.fitness,
-                    'steps': self.steps,
-                    }, path)
-        
+            'actor_init_dict': self.actor.init_dict,
+            'actor_state_dict': self.actor.state_dict(),
+            'actor_target_init_dict': self.actor_target.init_dict,
+            'actor_target_state_dict': self.actor_target.state_dict(),
+            'critic_init_dict': self.critic.init_dict,
+            'critic_state_dict': self.critic.state_dict(),
+            'critic_target_init_dict': self.critic_target.init_dict,
+            'critic_target_state_dict': self.critic_target.state_dict(),
+            'actor_optimizer_state_dict': self.actor_optimizer.state_dict(),
+            'critic_optimizer_state_dict': self.critic_optimizer.state_dict(),
+            'net_config': self.net_config,
+            'batch_size': self.batch_size,
+            'lr': self.lr,
+            'learn_step': self.learn_step,
+            'gamma': self.gamma,
+            'tau': self.tau,
+            'mutation': self.mut,
+            'index': self.index,
+            'scores': self.scores,
+            'fitness': self.fitness,
+            'steps': self.steps,
+        }, path)
+
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
         checkpoint = torch.load(path)
         self.net_config = checkpoint['net_config']
         if self.net_config['arch'] == 'mlp':
             self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableMLP(
+                **checkpoint['actor_target_init_dict'])
             self.critic = EvolvableMLP(**checkpoint['critic_init_dict'])
-            self.critic_target = EvolvableMLP(**checkpoint['critic_target_init_dict'])
+            self.critic_target = EvolvableMLP(
+                **checkpoint['critic_target_init_dict'])
         elif self.net_config['arch'] == 'cnn':
             self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableCNN(
+                **checkpoint['actor_target_init_dict'])
             self.critic = EvolvableCNN(**checkpoint['critic_init_dict'])
-            self.critic_target = EvolvableCNN(**checkpoint['critic_target_init_dict'])
+            self.critic_target = EvolvableCNN(
+                **checkpoint['critic_target_init_dict'])
         self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
+        self.actor_target.load_state_dict(
+            checkpoint['actor_target_state_dict'])
         self.critic.load_state_dict(checkpoint['critic_state_dict'])
-        self.critic_target.load_state_dict(checkpoint['critic_target_state_dict'])
-        self.actor_optimizer.load_state_dict(checkpoint['actor_optimizer_state_dict'])
-        self.critic_optimizer.load_state_dict(checkpoint['critic_optimizer_state_dict'])
+        self.critic_target.load_state_dict(
+            checkpoint['critic_target_state_dict'])
+        self.actor_optimizer.load_state_dict(
+            checkpoint['actor_optimizer_state_dict'])
+        self.critic_optimizer.load_state_dict(
+            checkpoint['critic_optimizer_state_dict'])
         self.batch_size = checkpoint['batch_size']
         self.lr = checkpoint['lr']
         self.learn_step = checkpoint['learn_step']
         self.gamma = checkpoint['gamma']
         self.tau = checkpoint['tau']
         self.mut = checkpoint['mutation']
         self.index = checkpoint['index']
         self.scores = checkpoint['scores']
         self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+        self.steps = checkpoint['steps']
```

### Comparing `agilerl-0.1.4/agilerl/algorithms/dqn.py` & `agilerl-0.1.5/agilerl/algorithms/dqn.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from agilerl.networks.evolvable_mlp import EvolvableMLP
 from agilerl.networks.evolvable_cnn import EvolvableCNN
 
+
 class DQN():
     """The DQN algorithm class. DQN paper: https://arxiv.org/abs/1312.5602
 
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
@@ -31,16 +32,33 @@
     :param tau: For soft update of target network parameters, defaults to 1e-3
     :type tau: float, optional
     :param mutation: Most recent mutation to agent, defaults to None
     :type mutation: str, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
-    def __init__(self, state_dim, action_dim, one_hot, index=0, net_config={'arch':'mlp','h_size':[64,64]}, batch_size=64, 
-                 lr=1e-4, learn_step=5, gamma=0.99, tau=1e-3, mutation=None, device='cpu'):
+
+    def __init__(
+        self,
+        state_dim,
+        action_dim,
+        one_hot,
+        index=0,
+        net_config={
+            'arch': 'mlp',
+            'h_size': [
+            64,
+            64]},
+            batch_size=64,
+            lr=1e-4,
+            learn_step=5,
+            gamma=0.99,
+            tau=1e-3,
+            mutation=None,
+            device='cpu'):
         self.algo = 'DQN'
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.one_hot = one_hot
         self.net_config = net_config
         self.batch_size = batch_size
         self.lr = lr
@@ -53,23 +71,47 @@
         self.index = index
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
         # model
         if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
-            self.actor = EvolvableMLP(num_inputs=state_dim[0], num_outputs=action_dim, hidden_size=self.net_config['h_size'], device=self.device).to(self.device)
-            self.actor_target = EvolvableMLP(num_inputs=state_dim[0], num_outputs=action_dim, hidden_size=self.net_config['h_size'], device=self.device).to(self.device)
+            self.actor = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config['h_size'],
+                device=self.device).to(
+                self.device)
+            self.actor_target = EvolvableMLP(
+                num_inputs=state_dim[0],
+                num_outputs=action_dim,
+                hidden_size=self.net_config['h_size'],
+                device=self.device).to(
+                self.device)
             self.actor_target.load_state_dict(self.actor.state_dict())
 
         elif self.net_config['arch'] == 'cnn':    # Convolutional Neural Network
-            self.actor = EvolvableCNN(input_shape=state_dim, num_actions=action_dim, channel_size=self.net_config['c_size'], kernal_size=self.net_config['k_size'],
-                                      stride_size=self.net_config['s_size'], hidden_size=self.net_config['h_size'], device=self.device).to(self.device)
-            self.actor_target = EvolvableCNN(input_shape=state_dim, num_actions=action_dim, channel_size=self.net_config['c_size'], kernal_size=self.net_config['k_size'],
-                                             stride_size=self.net_config['s_size'], hidden_size=self.net_config['h_size'], device=self.device).to(self.device)
+            self.actor = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config['c_size'],
+                kernal_size=self.net_config['k_size'],
+                stride_size=self.net_config['s_size'],
+                hidden_size=self.net_config['h_size'],
+                device=self.device).to(
+                self.device)
+            self.actor_target = EvolvableCNN(
+                input_shape=state_dim,
+                num_actions=action_dim,
+                channel_size=self.net_config['c_size'],
+                kernal_size=self.net_config['k_size'],
+                stride_size=self.net_config['s_size'],
+                hidden_size=self.net_config['h_size'],
+                device=self.device).to(
+                self.device)
             self.actor_target.load_state_dict(self.actor.state_dict())
 
         self.optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
         self.criterion = nn.MSELoss()
 
     def getAction(self, state, epsilon=0):
         """Returns the next action to take in the environment. Epsilon is the probability of taking a random action, used for exploration.
@@ -79,62 +121,70 @@
         :type state: float or List[float]
         :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
         :type epsilon: float, optional
         """
         state = torch.from_numpy(state).float().to(self.device)
 
         if self.one_hot:
-            state = nn.functional.one_hot(state.long(), num_classes=self.state_dim[0]).float().squeeze()
-        
-        if len(state.size())<2:
+            state = nn.functional.one_hot(
+                state.long(), num_classes=self.state_dim[0]).float().squeeze()
+
+        if len(state.size()) < 2:
             state = state.unsqueeze(0)
 
         self.actor.eval()
         with torch.no_grad():
             action_values = self.actor(state)
         self.actor.train()
 
         # epsilon-greedy
         if random.random() < epsilon:
-            action = np.random.randint(0, self.action_dim, size=state.size()[0])
+            action = np.random.randint(
+                0, self.action_dim, size=state.size()[0])
         else:
             action = np.argmax(action_values.cpu().data.numpy(), axis=1)
 
         return action
 
     def learn(self, experiences):
         """Updates agent network parameters to learn from experiences.
 
         :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
         :type state: List[torch.Tensor[float]]
         """
         states, actions, rewards, next_states, dones = experiences
 
         if self.one_hot:
-            states = nn.functional.one_hot(states.long(), num_classes=self.state_dim[0]).float().squeeze()
-            next_states = nn.functional.one_hot(next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
-
-        q_target = self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
-        y_j = rewards + self.gamma * q_target * (1 - dones)          # target, if terminal then y_j = rewards
+            states = nn.functional.one_hot(
+                states.long(), num_classes=self.state_dim[0]).float().squeeze()
+            next_states = nn.functional.one_hot(
+                next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
+
+        q_target = self.actor_target(next_states).detach().max(axis=1)[
+            0].unsqueeze(1)
+        # target, if terminal then y_j = rewards
+        y_j = rewards + self.gamma * q_target * (1 - dones)
         q_eval = self.actor(states).gather(1, actions.long())
 
         # loss backprop
         loss = self.criterion(q_eval, y_j)
         self.optimizer.zero_grad()
         loss.backward()
         self.optimizer.step()
 
         # soft update target network
         self.softUpdate()
 
     def softUpdate(self):
         """Soft updates target network.
         """
-        for eval_param, target_param in zip(self.actor.parameters(), self.actor_target.parameters()):
-            target_param.data.copy_(self.tau*eval_param.data + (1.0-self.tau)*target_param.data)
+        for eval_param, target_param in zip(
+                self.actor.parameters(), self.actor_target.parameters()):
+            target_param.data.copy_(
+                self.tau * eval_param.data + (1.0 - self.tau) * target_param.data)
 
     def test(self, env, swap_channels=False, max_steps=500, loop=3):
         """Returns mean test score of agent in environment with epsilon-greedy policy.
 
         :param env: The environment to be tested in
         :type env: Gym-style environment
         :param swap_channels: Swap image channels dimension from last to first [H, W, C] -> [C, H, W], defaults to False
@@ -166,81 +216,84 @@
         :param index: Index to keep track of agent for tournament selection and mutation, defaults to None
         :type index: int, optional
         """
         if index is None:
             index = self.index
 
         clone = type(self)(state_dim=self.state_dim,
-                            action_dim=self.action_dim,
-                            one_hot=self.one_hot,
-                            index=index, 
-                            net_config = self.net_config, 
-                            batch_size=self.batch_size,
-                            lr=self.lr,
-                            learn_step=self.learn_step,
-                            gamma=self.gamma,
-                            tau=self.tau,
-                            mutation=self.mut,
-                            device=self.device,
+                           action_dim=self.action_dim,
+                           one_hot=self.one_hot,
+                           index=index,
+                           net_config=self.net_config,
+                           batch_size=self.batch_size,
+                           lr=self.lr,
+                           learn_step=self.learn_step,
+                           gamma=self.gamma,
+                           tau=self.tau,
+                           mutation=self.mut,
+                           device=self.device,
                            )
-                           
+
         clone.actor = self.actor.clone().to(self.device)
         clone.actor_target = self.actor_target.clone().to(self.device)
         clone.optimizer = optim.Adam(clone.actor.parameters(), lr=clone.lr)
         clone.fitness = copy.deepcopy(self.fitness)
         clone.steps = copy.deepcopy(self.steps)
         clone.scores = copy.deepcopy(self.scores)
 
         return clone
-    
+
     def saveCheckpoint(self, path):
         """Saves a checkpoint of agent properties and network weights to path.
 
         :param path: Location to save checkpoint at
         :type path: string
         """
         torch.save({
-                    'actor_init_dict': self.actor.init_dict,
-                    'actor_state_dict': self.actor.state_dict(),
-                    'actor_target_init_dict': self.actor_target.init_dict,
-                    'actor_target_state_dict': self.actor_target.state_dict(),
-                    'optimizer_state_dict': self.optimizer.state_dict(),
-                    'net_config': self.net_config,
-                    'batch_size': self.batch_size,
-                    'lr': self.lr,
-                    'learn_step': self.learn_step,
-                    'gamma': self.gamma,
-                    'tau': self.tau,
-                    'mutation': self.mut,
-                    'index': self.index, 
-                    'scores': self.scores,
-                    'fitness': self.fitness,
-                    'steps': self.steps,
-                    }, path)
-        
+            'actor_init_dict': self.actor.init_dict,
+            'actor_state_dict': self.actor.state_dict(),
+            'actor_target_init_dict': self.actor_target.init_dict,
+            'actor_target_state_dict': self.actor_target.state_dict(),
+            'optimizer_state_dict': self.optimizer.state_dict(),
+            'net_config': self.net_config,
+            'batch_size': self.batch_size,
+            'lr': self.lr,
+            'learn_step': self.learn_step,
+            'gamma': self.gamma,
+            'tau': self.tau,
+            'mutation': self.mut,
+            'index': self.index,
+            'scores': self.scores,
+            'fitness': self.fitness,
+            'steps': self.steps,
+        }, path)
+
     def loadCheckpoint(self, path):
         """Loads saved agent properties and network weights from checkpoint.
 
         :param path: Location to load checkpoint from
         :type path: string
         """
         checkpoint = torch.load(path)
         self.net_config = checkpoint['net_config']
         if self.net_config['arch'] == 'mlp':
             self.actor = EvolvableMLP(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableMLP(**checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableMLP(
+                **checkpoint['actor_target_init_dict'])
         elif self.net_config['arch'] == 'cnn':
             self.actor = EvolvableCNN(**checkpoint['actor_init_dict'])
-            self.actor_target = EvolvableCNN(**checkpoint['actor_target_init_dict'])
+            self.actor_target = EvolvableCNN(
+                **checkpoint['actor_target_init_dict'])
         self.actor.load_state_dict(checkpoint['actor_state_dict'])
-        self.actor_target.load_state_dict(checkpoint['actor_target_state_dict'])
+        self.actor_target.load_state_dict(
+            checkpoint['actor_target_state_dict'])
         self.optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
         self.batch_size = checkpoint['batch_size']
         self.lr = checkpoint['lr']
         self.learn_step = checkpoint['learn_step']
         self.gamma = checkpoint['gamma']
         self.tau = checkpoint['tau']
         self.mut = checkpoint['mutation']
         self.index = checkpoint['index']
         self.scores = checkpoint['scores']
         self.fitness = checkpoint['fitness']
-        self.steps = checkpoint['steps']
+        self.steps = checkpoint['steps']
```

### Comparing `agilerl-0.1.4/agilerl/benchmarking.py` & `agilerl-0.1.5/agilerl/benchmarking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,81 +1,95 @@
 import torch
-import gymnasium as gym
 
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
-from agilerl.utils import makeVectEnvs, initialPopulation, printHyperparams, plotPopulationScore
+from agilerl.utils.utils import makeVectEnvs, initialPopulation, printHyperparams
 from agilerl.training.train import train
 
+
 def main(INIT_HP, MUTATION_PARAMS, NET_CONFIG):
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     print('============ AgileRL ============')
     print(f'DEVICE: {device}')
 
     env = makeVectEnvs(INIT_HP['ENV_NAME'], num_envs=16)
     try:
         state_dim = env.single_observation_space.n
         one_hot = True
-    except:
+    except BaseException:
         state_dim = env.single_observation_space.shape
         one_hot = False
     try:
         action_dim = env.single_action_space.n
-    except:
+    except BaseException:
         action_dim = env.single_action_space.shape[0]
 
     if INIT_HP['CHANNELS_LAST']:
         state_dim = (state_dim[2], state_dim[0], state_dim[1])
 
     field_names = ["state", "action", "reward", "next_state", "done"]
-    memory = ReplayBuffer(action_dim, INIT_HP['MEMORY_SIZE'], field_names=field_names, device=device)
-    tournament = TournamentSelection(INIT_HP['TOURN_SIZE'], INIT_HP['ELITISM'], INIT_HP['POP_SIZE'], INIT_HP['EVO_EPOCHS'])
+    memory = ReplayBuffer(
+        action_dim, INIT_HP['MEMORY_SIZE'], field_names=field_names, device=device)
+    tournament = TournamentSelection(
+        INIT_HP['TOURN_SIZE'],
+        INIT_HP['ELITISM'],
+        INIT_HP['POP_SIZE'],
+        INIT_HP['EVO_EPOCHS'])
     mutations = Mutations(algo=INIT_HP['ALGO'],
-                        no_mutation=MUTATION_PARAMS['NO_MUT'], 
-                        architecture=MUTATION_PARAMS['ARCH_MUT'], 
-                        new_layer_prob=MUTATION_PARAMS['NEW_LAYER'], 
-                        parameters=MUTATION_PARAMS['PARAMS_MUT'], 
-                        activation=MUTATION_PARAMS['ACT_MUT'], 
-                        rl_hp=MUTATION_PARAMS['RL_HP_MUT'], 
-                        rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], 
-                        mutation_sd=MUTATION_PARAMS['MUT_SD'], 
-                        arch=NET_CONFIG['arch'],
-                        rand_seed=MUTATION_PARAMS['RAND_SEED'],
-                        device=device)
-
-    agent_pop = initialPopulation(INIT_HP['ALGO'], state_dim, action_dim, one_hot, NET_CONFIG, INIT_HP, INIT_HP['POP_SIZE'], device=device)
+                          no_mutation=MUTATION_PARAMS['NO_MUT'],
+                          architecture=MUTATION_PARAMS['ARCH_MUT'],
+                          new_layer_prob=MUTATION_PARAMS['NEW_LAYER'],
+                          parameters=MUTATION_PARAMS['PARAMS_MUT'],
+                          activation=MUTATION_PARAMS['ACT_MUT'],
+                          rl_hp=MUTATION_PARAMS['RL_HP_MUT'],
+                          rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],
+                          mutation_sd=MUTATION_PARAMS['MUT_SD'],
+                          arch=NET_CONFIG['arch'],
+                          rand_seed=MUTATION_PARAMS['RAND_SEED'],
+                          device=device)
 
-    trained_pop, pop_fitnesses = train(env,
-        INIT_HP['ENV_NAME'],
+    agent_pop = initialPopulation(
         INIT_HP['ALGO'],
-        agent_pop,
-        memory=memory,
-        swap_channels=INIT_HP['CHANNELS_LAST'],
-        n_episodes=INIT_HP['EPISODES'],
-        evo_epochs=INIT_HP['EVO_EPOCHS'],
-        evo_loop=1,
-        target=INIT_HP['TARGET_SCORE'],
-        tournament=tournament,
-        mutation=mutations,
-        wb=INIT_HP['WANDB'],
+        state_dim,
+        action_dim,
+        one_hot,
+        NET_CONFIG,
+        INIT_HP,
+        INIT_HP['POP_SIZE'],
         device=device)
 
+    trained_pop, pop_fitnesses = train(env,
+                                       INIT_HP['ENV_NAME'],
+                                       INIT_HP['ALGO'],
+                                       agent_pop,
+                                       memory=memory,
+                                       swap_channels=INIT_HP['CHANNELS_LAST'],
+                                       n_episodes=INIT_HP['EPISODES'],
+                                       evo_epochs=INIT_HP['EVO_EPOCHS'],
+                                       evo_loop=1,
+                                       target=INIT_HP['TARGET_SCORE'],
+                                       tournament=tournament,
+                                       mutation=mutations,
+                                       wb=INIT_HP['WANDB'],
+                                       device=device)
+
     printHyperparams(trained_pop)
     # plotPopulationScore(trained_pop)
 
     if str(device) == "cuda":
         torch.cuda.empty_cache()
 
 
 if __name__ == '__main__':
     INIT_HP = {
         'ENV_NAME': 'LunarLander-v2',   # Gym environment name
         'ALGO': 'DQN',                  # Algorithm
-        'CHANNELS_LAST': False,         # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+        # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+        'CHANNELS_LAST': False,
         'BATCH_SIZE': 256,              # Batch size
         'LR': 1e-3,                     # Learning rate
         'EPISODES': 2000,               # Max no. episodes
         'TARGET_SCORE': 200.,           # Early training stop at avg score of last 100 episodes
         'GAMMA': 0.99,                  # Discount factor
         'MEMORY_SIZE': 10000,           # Max memory buffer size
         'LEARN_STEP': 1,                # Learning frequency
@@ -91,18 +105,19 @@
     MUTATION_PARAMS = {  # Relative probabilities
         'NO_MUT': 0.4,                              # No mutation
         'ARCH_MUT': 0.2,                            # Architecture mutation
         'NEW_LAYER': 0.2,                           # New layer mutation
         'PARAMS_MUT': 0.2,                          # Network parameters mutation
         'ACT_MUT': 0,                               # Activation layer mutation
         'RL_HP_MUT': 0.2,                           # Learning HP mutation
-        'RL_HP_SELECTION': ['lr', 'batch_size'],    # Learning HPs to choose from
+        # Learning HPs to choose from
+        'RL_HP_SELECTION': ['lr', 'batch_size'],
         'MUT_SD': 0.1,                              # Mutation strength
         'RAND_SEED': 1,                             # Random seed
     }
 
     NET_CONFIG = {
         'arch': 'mlp',      # Network architecture
         'h_size': [32, 32],    # Actor hidden size
     }
 
-    main(INIT_HP, MUTATION_PARAMS, NET_CONFIG)
+    main(INIT_HP, MUTATION_PARAMS, NET_CONFIG)
```

### Comparing `agilerl-0.1.4/agilerl/components/replay_buffer.py` & `agilerl-0.1.5/agilerl/components/replay_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import torch
 import numpy as np
 from collections import deque, namedtuple
 import random
 
+
 class ReplayBuffer():
     """The Experience Replay Buffer class. Used to store experiences and allow off-policy learning.
 
     :param n_actions: Action dimension
     :type n_actions: int
     :param memory_size: Maximum length of replay buffer
     :type memory_size: int
     :param field_names: Field names for experience named tuple, e.g. ['state', 'action', 'reward']
     :type field_names: List[str]
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
+
     def __init__(self, action_dim, memory_size, field_names, device='cpu'):
         self.n_actions = action_dim
-        self.memory = deque(maxlen = memory_size)
+        self.memory = deque(maxlen=memory_size)
         self.experience = namedtuple("Experience", field_names=field_names)
         self.counter = 0    # update cycle counter
         self.device = device
 
     def __len__(self):
         return len(self.memory)
 
@@ -33,19 +35,24 @@
         """Returns sample of experiences from memory.
 
         :param batch_size: Number of samples to return
         :type batch_size: int
         """
         experiences = random.sample(self.memory, k=batch_size)
 
-        states = torch.from_numpy(np.stack([e.state for e in experiences if e is not None], axis=0)).to(self.device)
-        actions = torch.from_numpy(np.vstack([e.action for e in experiences if e is not None])).to(self.device)
-        rewards = torch.from_numpy(np.vstack([e.reward for e in experiences if e is not None])).float().to(self.device)
-        next_states = torch.from_numpy(np.stack([e.next_state for e in experiences if e is not None], axis=0)).float().to(self.device)
-        dones = torch.from_numpy(np.vstack([e.done for e in experiences if e is not None]).astype(np.uint8)).float().to(self.device)
+        states = torch.from_numpy(np.stack(
+            [e.state for e in experiences if e is not None], axis=0)).to(self.device)
+        actions = torch.from_numpy(
+            np.vstack([e.action for e in experiences if e is not None])).to(self.device)
+        rewards = torch.from_numpy(np.vstack(
+            [e.reward for e in experiences if e is not None])).float().to(self.device)
+        next_states = torch.from_numpy(np.stack(
+            [e.next_state for e in experiences if e is not None], axis=0)).float().to(self.device)
+        dones = torch.from_numpy(np.vstack([e.done for e in experiences if e is not None]).astype(
+            np.uint8)).float().to(self.device)
 
         return (states, actions, rewards, next_states, dones)
 
     def save2memory(self, state, action, reward, next_state, done):
         """Saves experience to memory.
 
         :param state: Environment observation
@@ -53,15 +60,15 @@
         :param action: Action in environment
         :type action: float or List[float]
         :param reward: Reward from environment
         :type reward: float
         :param next_state: Environment observation of next state
         :type next_state: float or List[float]
         :param done: True if environment episode finished, else False
-        :type done: bool 
+        :type done: bool
         """
         self._add(state, action, reward, next_state, done)
         self.counter += 1
 
     def save2memoryVectEnvs(self, states, actions, rewards, next_states, dones):
         """Saves multiple experiences to memory.
 
@@ -72,10 +79,11 @@
         :param rewards: Multiple rewards from environment in a batch
         :type rewards: List[float]
         :param next_states: Multiple environment observations of next states in a batch
         :type next_states: List[float] or List[List[float]]
         :param dones: True if environment episodes finished, else False, in a batch
         :type dones: List[bool]
         """
-        for state, action, reward, next_state, done in zip(states, actions, rewards, next_states, dones):
+        for state, action, reward, next_state, done in zip(
+                states, actions, rewards, next_states, dones):
             self._add(state, action, reward, next_state, done)
-            self.counter += 1
+            self.counter += 1
```

### Comparing `agilerl-0.1.4/agilerl/hpo/mutation.py` & `agilerl-0.1.5/agilerl/hpo/mutation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import torch.optim as optim
 import numpy as np
 import fastrand
 
+
 class Mutations():
     """The Mutations class for evolutionary hyperparameter optimization.
 
     :param algo: RL algorithm used. Use str e.g. 'DQN' if using AgileRL implementation of algorithm, or provide a dict with names of agent networks
     :type algo: str or dict
     :param no_mutation: Relative probability of no mutation
     :type no_mutation: float
@@ -26,56 +26,73 @@
     :param arch: Network architecture type. 'mlp' or 'cnn', defaults to 'mlp'
     :type arch: str, optional
     :param rand_seed: Random seed for repeatability, defaults to None
     :type rand_seed: int, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
-    def __init__(self, algo, no_mutation, architecture, new_layer_prob, parameters, activation, rl_hp, rl_hp_selection, mutation_sd, arch='mlp', rand_seed=None, device='cpu'):
-        self.rng = np.random.RandomState(rand_seed) # Random seed for repeatability
+
+    def __init__(
+            self,
+            algo,
+            no_mutation,
+            architecture,
+            new_layer_prob,
+            parameters,
+            activation,
+            rl_hp,
+            rl_hp_selection,
+            mutation_sd,
+            arch='mlp',
+            rand_seed=None,
+            device='cpu'):
+        # Random seed for repeatability
+        self.rng = np.random.RandomState(rand_seed)
 
         self.arch = arch    # Network architecture type
-        
+
         # Relative probabilities of mutation
         self.no_mut = no_mutation               # No mutation
         self.architecture_mut = architecture    # Architecture mutation
-        self.new_layer_prob = new_layer_prob    # New layer mutation (type of architecture mutation)
+        # New layer mutation (type of architecture mutation)
+        self.new_layer_prob = new_layer_prob
         self.parameters_mut = parameters        # Network parameters mutation
         self.activation_mut = activation        # Activation layer mutation
         self.rl_hp_mut = rl_hp                  # Learning HP mutation
-        
+
         self.rl_hp_selection = rl_hp_selection  # Learning HPs to choose from
         self.mutation_sd = mutation_sd          # Mutation strength
 
         # Set algorithm dictionary with agent network names for mutation
         # Use custom agent dict, or pre-configured agent from API
-        if type(algo) is dict:
+        if isinstance(algo, dict):
             self.algo = algo
         else:
             self.algo = self.get_algo_nets(algo)
 
         self.device = device
 
     def no_mutation(self, individual):
         """Returns individual from population without mutation.
-        
+
         :param individual: Individual agent from population
         :type individual: object
         """
-        individual.mut = 'None' # No mutation
+        individual.mut = 'None'  # No mutation
         return individual
 
     # Generic mutation function - gather mutation options and select from these
     def mutation(self, population):
         """Returns mutated population.
 
         :param population: Population of agents
         :type population: List[object]
         """
-        # Create lists of possible mutation functions and their respective relative probabilities
+        # Create lists of possible mutation functions and their respective
+        # relative probabilities
         mutation_options = []
         mutation_proba = []
         if self.no_mut:
             mutation_options.append(self.no_mutation)
             mutation_proba.append(float(self.no_mut))
         if self.architecture_mut:
             mutation_options.append(self.architecture_mutate)
@@ -86,223 +103,254 @@
         if self.activation_mut:
             mutation_options.append(self.activation_mutation)
             mutation_proba.append(float(self.activation_mut))
         if self.rl_hp_mut:
             mutation_options.append(self.rl_hyperparam_mutation)
             mutation_proba.append(float(self.rl_hp_mut))
 
-        if len(mutation_options) == 0: # Return if no mutation options
+        if len(mutation_options) == 0:  # Return if no mutation options
             return population
 
-        mutation_proba = np.array(mutation_proba) / np.sum(mutation_proba) # Normalize probs
+        mutation_proba = np.array(mutation_proba) / \
+            np.sum(mutation_proba)  # Normalize probs
 
-        # Raandomly choose mutation for each agent in population from options with relative probabilities
-        mutation_choice = self.rng.choice(mutation_options, len(population), p=mutation_proba)
+        # Raandomly choose mutation for each agent in population from options with
+        # relative probabilities
+        mutation_choice = self.rng.choice(
+            mutation_options, len(population), p=mutation_proba)
 
         mutated_population = []
         for mutation, individual in zip(mutation_choice, population):
 
-            individual = mutation(individual)   # Call mutation function for each individual
+            # Call mutation function for each individual
+            individual = mutation(individual)
 
             offspring_actor = getattr(individual, self.algo['actor']['eval'])
-                        
-            # Reinitialise target network with frozen weights due to potential mutation in architecture of value network
+
+            # Reinitialise target network with frozen weights due to potential
+            # mutation in architecture of value network
             ind_target = type(offspring_actor)(**offspring_actor.init_dict)
             ind_target.load_state_dict(offspring_actor.state_dict())
-            setattr(individual, self.algo['actor']['target'], ind_target.to(self.device))
+            setattr(individual, self.algo['actor']
+                    ['target'], ind_target.to(self.device))
 
-            # If algorithm has critics, reinitialize their respective target networks too
+            # If algorithm has critics, reinitialize their respective target networks
+            # too
             for critic in self.algo['critics']:
                 offspring_critic = getattr(individual, critic['eval'])
-                ind_target = type(offspring_critic)(**offspring_critic.init_dict)
+                ind_target = type(offspring_critic)(
+                    **offspring_critic.init_dict)
                 ind_target.load_state_dict(offspring_critic.state_dict())
-                setattr(individual, critic['target'], ind_target.to(self.device))
+                setattr(individual, critic['target'],
+                        ind_target.to(self.device))
 
             mutated_population.append(individual)
 
         return mutated_population
 
     def rl_hyperparam_mutation(self, individual):
         """Returns individual from population with RL hyperparameter mutation.
-        
+
         :param individual: Individual agent from population
         :type individual: object
         """
         # Learning hyperparameter mutation
         rl_params = self.rl_hp_selection
-        mutate_param = self.rng.choice(rl_params, 1)[0] # Select HP to mutate from options
+        # Select HP to mutate from options
+        mutate_param = self.rng.choice(rl_params, 1)[0]
 
         # Increase or decrease HP randomly (within clipped limits)
         random_num = self.rng.uniform(0, 1)
         if mutate_param == 'batch_size':
             if random_num > 0.5:
-                individual.batch_size = min(128, max(8, int(individual.batch_size * 1.2)))
+                individual.batch_size = min(
+                    128, max(8, int(individual.batch_size * 1.2)))
             else:
-                individual.batch_size = min(128, max(8, int(individual.batch_size * 0.8)))
+                individual.batch_size = min(
+                    128, max(8, int(individual.batch_size * 0.8)))
             individual.mut = 'bs'
 
         elif mutate_param == 'lr':
             if random_num > 0.5:
                 individual.lr = min(0.005, max(0.00001, individual.lr * 1.2))
             else:
                 individual.lr = min(0.005, max(0.00001, individual.lr * 0.8))
-            
+
             # Reinitialise optimizer if new learning rate
             actor_opt = getattr(individual, self.algo['actor']['optimizer'])
-            net_params = getattr(individual, self.algo['actor']['eval']).parameters()
-            setattr(individual, self.algo['actor']['optimizer'], type(actor_opt)(net_params, lr=individual.lr))
-            
+            net_params = getattr(
+                individual, self.algo['actor']['eval']).parameters()
+            setattr(individual, self.algo['actor']['optimizer'], type(
+                actor_opt)(net_params, lr=individual.lr))
+
             # If algorithm has critics, reinitialise their optimizers too
             for critic in self.algo['critics']:
                 critic_opt = getattr(individual, critic['optimizer'])
                 net_params = getattr(individual, critic['eval']).parameters()
-                setattr(individual, critic['optimizer'], type(critic_opt)(net_params, lr=individual.lr)) 
+                setattr(individual, critic['optimizer'], type(
+                    critic_opt)(net_params, lr=individual.lr))
             individual.mut = 'lr'
 
         elif mutate_param == 'learn_step':
             if random_num > 0.5:
-                individual.learn_step = min(1, max(0, int(individual.learn_step * 1.5)))
+                individual.learn_step = min(
+                    1, max(0, int(individual.learn_step * 1.5)))
             else:
-                individual.learn_step = min(1, max(0, int(individual.learn_step * 0.75)))
+                individual.learn_step = min(
+                    1, max(0, int(individual.learn_step * 0.75)))
 
         return individual
 
     def activation_mutation(self, individual):
         """Returns individual from population with activation layer mutation.
-        
+
         :param individual: Individual agent from population
         :type individual: object
         """
         if individual.algo == 'DDPG':   # Needs to stay tanh for DDPG continuous actions
             individual.mut = 'None'
             return individual
-        
+
         # Mutate network activation layer
         offspring_actor = getattr(individual, self.algo['actor']['eval'])
-        offspring_actor = self._permutate_activation(offspring_actor)   # Mutate activation function
-        setattr(individual, self.algo['actor']['eval'], offspring_actor.to(self.device))
+        offspring_actor = self._permutate_activation(
+            offspring_actor)   # Mutate activation function
+        setattr(individual, self.algo['actor']
+                ['eval'], offspring_actor.to(self.device))
 
         # If algorithm has critics, mutate their activations too
         for critic in self.algo['critics']:
             offspring_critic = getattr(individual, critic['eval'])
             offspring_critic = self._permutate_activation(offspring_critic)
-            setattr(individual, critic['eval'], offspring_critic.to(self.device))
-        
+            setattr(individual, critic['eval'],
+                    offspring_critic.to(self.device))
+
         individual.mut = 'act'
         return individual
 
     def _permutate_activation(self, network):
         # Function to change network activation layer
         possible_activations = ['relu', 'elu', 'gelu']
         if self.arch == 'cnn':
             current_activation = network.mlp_activation
         else:   # mlp
             current_activation = network.activation
-        # Remove current activation from options to ensure different new activation layer
+        # Remove current activation from options to ensure different new
+        # activation layer
         possible_activations.remove(current_activation)
-        new_activation = self.rng.choice(possible_activations, size=1)[0]   # Select new activation
+        new_activation = self.rng.choice(possible_activations, size=1)[
+            0]   # Select new activation
         net_dict = network.init_dict
         if self.arch == 'cnn':
             net_dict['mlp_activation'] = new_activation
             net_dict['cnn_activation'] = new_activation
-        else:   # mlp
+        else:   # mlp, gpt or bert
             net_dict['activation'] = new_activation
         new_network = type(network)(**net_dict)
         new_network.load_state_dict(network.state_dict())
         network = new_network
 
         return network.to(self.device)
 
     def parameter_mutation(self, individual):
         """Returns individual from population with network parameters mutation.
-        
+
         :param individual: Individual agent from population
         :type individual: object
         """
         # Mutate network parameters
         offspring_actor = getattr(individual, self.algo['actor']['eval'])
-        offspring_actor = self.classic_parameter_mutation(offspring_actor) # Network parameter mutation function
-        setattr(individual, self.algo['actor']['eval'], offspring_actor.to(self.device))
+        offspring_actor = self.classic_parameter_mutation(
+            offspring_actor)  # Network parameter mutation function
+        setattr(individual, self.algo['actor']
+                ['eval'], offspring_actor.to(self.device))
         individual.mut = 'param'
         return individual
 
     def regularize_weight(self, weight, mag):
-        if weight > mag: weight = mag
-        if weight < -mag: weight = -mag
+        if weight > mag:
+            weight = mag
+        if weight < -mag:
+            weight = -mag
         return weight
 
     def classic_parameter_mutation(self, network):
         """Returns network with mutated weights.
-        
+
         :param network: Neural network to mutate
         :type individual: torch.nn.Module
         """
         # Function to mutate network weights with Gaussian noise
         mut_strength = self.mutation_sd
         num_mutation_frac = 0.1
         super_mut_strength = 10
         super_mut_prob = 0.05
         reset_prob = super_mut_prob + 0.05
 
         model_params = network.state_dict()
 
         potential_keys = []
         for i, key in enumerate(model_params):  # Mutate each param
-            if not 'norm' in key:
+            if 'norm' not in key:
                 W = model_params[key]
                 if len(W.shape) == 2:  # Weights, no bias
                     potential_keys.append(key)
 
         how_many = np.random.randint(1, len(potential_keys) + 1, 1)[0]
         chosen_keys = np.random.choice(potential_keys, how_many, replace=False)
 
         for key in chosen_keys:
             # References to the variable keys
             W = model_params[key]
             num_weights = W.shape[0] * W.shape[1]
             # Number of mutation instances
-            num_mutations = fastrand.pcg32bounded(int(np.ceil(num_mutation_frac * num_weights)))
+            num_mutations = fastrand.pcg32bounded(
+                int(np.ceil(num_mutation_frac * num_weights)))
             for _ in range(num_mutations):
                 ind_dim1 = fastrand.pcg32bounded(W.shape[0])
                 ind_dim2 = fastrand.pcg32bounded(W.shape[-1])
                 random_num = self.rng.uniform(0, 1)
 
                 if random_num < super_mut_prob:  # Super Mutation probability
-                    W[ind_dim1, ind_dim2] += self.rng.normal(0, np.abs(super_mut_strength * W[ind_dim1, ind_dim2].item()))
+                    W[ind_dim1, ind_dim2] += self.rng.normal(
+                        0, np.abs(super_mut_strength * W[ind_dim1, ind_dim2].item()))
                 elif random_num < reset_prob:  # Reset probability
                     W[ind_dim1, ind_dim2] = self.rng.normal(0, 1)
                 else:  # mutauion even normal
-                    W[ind_dim1, ind_dim2] += self.rng.normal(0, np.abs(mut_strength * W[ind_dim1, ind_dim2].item()))
+                    W[ind_dim1, ind_dim2] += self.rng.normal(
+                        0, np.abs(mut_strength * W[ind_dim1, ind_dim2].item()))
 
                 # Regularization hard limit
-                W[ind_dim1, ind_dim2] = self.regularize_weight(W[ind_dim1, ind_dim2].item(), 1000000)
+                W[ind_dim1, ind_dim2] = self.regularize_weight(
+                    W[ind_dim1, ind_dim2].item(), 1000000)
         return network.to(self.device)
 
-
     def architecture_mutate(self, individual):
         """Returns individual from population with network architecture mutation.
-        
+
         :param individual: Individual agent from population
         :type individual: object
         """
         # Mutate network architecture by adding layers or nodes
-        offspring_actor = getattr(individual, self.algo['actor']['eval']).clone()
-        offspring_critics = [getattr(individual, critic['eval']).clone() for critic in self.algo['critics']]
+        offspring_actor = getattr(
+            individual, self.algo['actor']['eval']).clone()
+        offspring_critics = [getattr(individual, critic['eval']).clone()
+                             for critic in self.algo['critics']]
 
         rand_numb = self.rng.uniform(0, 1)
 
         # Randomly select whether to add layer or node with relative probabilities
         # If algorithm has critics, apply to these too
 
         if self.arch == 'cnn':
-            if rand_numb < self.new_layer_prob/2:
+            if rand_numb < self.new_layer_prob / 2:
                 offspring_actor.add_mlp_layer()
                 for offspring_critic in offspring_critics:
                     offspring_critic.add_mlp_layer()
-            elif self.new_layer_prob/2 <= rand_numb < self.new_layer_prob:
+            elif self.new_layer_prob / 2 <= rand_numb < self.new_layer_prob:
                 offspring_actor.add_cnn_layer()
                 for offspring_critic in offspring_critics:
                     offspring_critic.add_cnn_layer()
             else:
                 rand_numb = self.rng.uniform(0, 1)
                 if rand_numb < 0.2:
                     offspring_actor.change_cnn_kernal()
@@ -312,55 +360,105 @@
                     offspring_actor.add_cnn_channel()
                     for offspring_critic in offspring_critics:
                         offspring_critic.add_cnn_channel()
                 else:
                     offspring_actor.add_mlp_node()
                     for offspring_critic in offspring_critics:
                         offspring_critic.add_mlp_node()
-            
-        else:   # mlp            
+
+        elif self.arch == 'bert':
+            if rand_numb < self.new_layer_prob / 2:
+                if self.rng.uniform(0, 1) < 0.5:
+                    offspring_actor.add_encoder_layer()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.add_encoder_layer()
+                else:
+                    offspring_actor.remove_encoder_layer()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.remove_encoder_layer()
+            elif self.new_layer_prob / 2 <= rand_numb < self.new_layer_prob:
+                if self.rng.uniform(0, 1) < 0.5:
+                    offspring_actor.add_decoder_layer()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.add_decoder_layer()
+                else:
+                    offspring_actor.remove_decoder_layer()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.remove_decoder_layer()
+            else:
+                if self.rng.uniform(0, 1) < 0.5:
+                    node_dict = offspring_actor.add_node()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.add_node(**node_dict)
+                else:
+                    node_dict = offspring_actor.remove_node()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.remove_node(**node_dict)
+
+        else:   # mlp or gpt
             if rand_numb < self.new_layer_prob:
-                offspring_actor.add_layer()
-                for offspring_critic in offspring_critics:
-                    offspring_critic.add_layer()
+                if self.rng.uniform(0, 1) < 0.5:
+                    offspring_actor.add_layer()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.add_layer()
+                else:
+                    offspring_actor.remove_layer()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.remove_layer()
             else:
-                node_dict = offspring_actor.add_node()
-                for offspring_critic in offspring_critics:
-                    offspring_critic.add_node(**node_dict)
+                if self.rng.uniform(0, 1) < 0.5:
+                    node_dict = offspring_actor.add_node()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.add_node(**node_dict)
+                else:
+                    node_dict = offspring_actor.remove_node()
+                    for offspring_critic in offspring_critics:
+                        offspring_critic.remove_node(**node_dict)
 
-        setattr(individual, self.algo['actor']['eval'], offspring_actor.to(self.device))
+        setattr(individual, self.algo['actor']
+                ['eval'], offspring_actor.to(self.device))
         for offspring_critic, critic in zip(offspring_critics, self.algo['critics']):
-            setattr(individual, critic['eval'], offspring_critic.to(self.device))
-           
+            setattr(individual, critic['eval'],
+                    offspring_critic.to(self.device))
+
         individual.mut = 'arch'
         return individual
 
     def get_algo_nets(self, algo):
         """Returns dictionary with agent network names.
-        
+
         :param algo: RL algorithm
         :type algo: string
         """
         # Function to return dictionary with names of agent networks to allow mutation
         if algo == 'DQN':
             nets = {
                 'actor': {
                     'eval': 'actor',
                     'target': 'actor_target',
                     'optimizer': 'optimizer'
-                    },
+                },
                 'critics': []
             }
         elif algo == 'DDPG':
             nets = {
                 'actor': {
                     'eval': 'actor',
                     'target': 'actor_target',
                     'optimizer': 'actor_optimizer'
-                    },
+                },
                 'critics': [{
                     'eval': 'critic',
                     'target': 'critic_target',
                     'optimizer': 'critic_optimizer'
-                    }]
+                }]
+            }
+        elif algo == 'ILQL':
+            nets = {
+                'actor': {
+                    'eval': 'actor',
+                    'target': 'actor_target',
+                    'optimizer': 'optimizer'
+                },
+                'critics': []
             }
-        return nets
+        return nets
```

### Comparing `agilerl-0.1.4/agilerl/hpo/tournament.py` & `agilerl-0.1.5/agilerl/hpo/tournament.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import copy
 
+
 class TournamentSelection():
     """The tournament selection class.
-    
+
     :param tournament_size: Tournament selection size
     :type tournament_size: int
     :param elitism: Elitism in tournament selection
     :type elitism: bool
     :param population_size: Number of agents in population
     :type population_size: int
     :param evo_step: Number of most recent fitness scores to use in evaluation
@@ -17,40 +18,42 @@
     def __init__(self, tournament_size, elitism, population_size, evo_step):
         self.tournament_size = tournament_size
         self.elitism = elitism
         self.population_size = population_size
         self.evo_step = evo_step
 
     def _tournament(self, fitness_values):
-        selection = np.random.randint(0, len(fitness_values), size=self.tournament_size)
+        selection = np.random.randint(
+            0, len(fitness_values), size=self.tournament_size)
         selection_values = [fitness_values[i] for i in selection]
         winner = selection[np.argmax(selection_values)]
         return winner
 
     def select(self, population):
         """Returns best agent and new population of agents following tournament selection.
-        
+
         :param population: Population of agents
         :type population: List[object]
         """
-        last_fitness = [np.mean(indi.fitness[-self.evo_step:]) for indi in population]
+        last_fitness = [np.mean(indi.fitness[-self.evo_step:])
+                        for indi in population]
         rank = np.argsort(last_fitness).argsort()
 
         max_id = max([ind.index for ind in population])
 
         elite = copy.deepcopy([population[np.argsort(rank)[-1]]][0])
 
         new_population = []
-        if self.elitism: # keep top agent in population
+        if self.elitism:  # keep top agent in population
             new_population.append(elite.clone())
             selection_size = self.population_size - 1
         else:
             selection_size = self.population_size
 
         # select parents of next gen using tournament selection
         for idx in range(selection_size):
             max_id += 1
             actor_parent = population[self._tournament(rank)]
             new_individual = actor_parent.clone(max_id)
             new_population.append(new_individual)
 
-        return elite, new_population
+        return elite, new_population
```

### Comparing `agilerl-0.1.4/agilerl/networks/evolvable_cnn.py` & `agilerl-0.1.5/agilerl/networks/evolvable_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,43 +8,47 @@
 import torch.autograd as autograd
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 class NoisyLinear(nn.Module):
     """The Noisy Linear Neural Network class.
-    
+
     :param in_features: Input features size
     :type in_features: int
     :param out_features: Output features size
     :type out_features: int
     :param std_init: Standard deviation, defaults to 0.4
     :type std_init: float, optional
     """
+
     def __init__(self, in_features, out_features, std_init=0.4):
         super(NoisyLinear, self).__init__()
 
         self.in_features = in_features
         self.out_features = out_features
         self.std_init = std_init
 
-        self.weight_mu = nn.Parameter(torch.FloatTensor(out_features, in_features))
-        self.weight_sigma = nn.Parameter(torch.FloatTensor(out_features, in_features))
-        self.register_buffer('weight_epsilon', torch.FloatTensor(out_features, in_features))
+        self.weight_mu = nn.Parameter(
+            torch.FloatTensor(out_features, in_features))
+        self.weight_sigma = nn.Parameter(
+            torch.FloatTensor(out_features, in_features))
+        self.register_buffer(
+            'weight_epsilon', torch.FloatTensor(out_features, in_features))
 
         self.bias_mu = nn.Parameter(torch.FloatTensor(out_features))
         self.bias_sigma = nn.Parameter(torch.FloatTensor(out_features))
         self.register_buffer('bias_epsilon', torch.FloatTensor(out_features))
 
         self.reset_parameters()
         self.reset_noise()
 
     def forward(self, x):
         """Returns output of neural network.
-        
+
         :param x: Neural network input
         :type x: torch.Tensor()
         """
         weight_epsilon = self.weight_epsilon.to(x.device)
         bias_epsilon = self.bias_epsilon.to(x.device)
 
         if self.training:
@@ -58,18 +62,20 @@
 
     def reset_parameters(self):
         """Resets neural network parameters.
         """
         mu_range = 1 / math.sqrt(self.weight_mu.size(1))
 
         self.weight_mu.data.uniform_(-mu_range, mu_range)
-        self.weight_sigma.data.fill_(self.std_init / math.sqrt(self.weight_sigma.size(1)))
+        self.weight_sigma.data.fill_(
+            self.std_init / math.sqrt(self.weight_sigma.size(1)))
 
         self.bias_mu.data.uniform_(-mu_range, mu_range)
-        self.bias_sigma.data.fill_(self.std_init / math.sqrt(self.bias_sigma.size(0)))
+        self.bias_sigma.data.fill_(
+            self.std_init / math.sqrt(self.bias_sigma.size(0)))
 
     def reset_noise(self):
         """Resets neural network noise.
         """
         epsilon_in = self._scale_noise(self.in_features)
         epsilon_out = self._scale_noise(self.out_features)
 
@@ -85,15 +91,15 @@
         x = torch.randn(size)
         x = x.sign().mul(x.abs().sqrt())
         return x
 
 
 class EvolvableCNN(nn.Module):
     """The Evolvable Convolutional Neural Network class.
-    
+
     :param input_shape: Input shape
     :type input_shape: List[int]
     :param channel_size: CNN channel size
     :type channel_size: List[int]
     :param kernel_size: Comvolution kernel size
     :type kernel_size: List[int]
     :param stride_size: Convolution stride size
@@ -115,17 +121,31 @@
     :param rainbow: Using Rainbow DQN, defaults to False
     :type rainbow: bool, optional
     :param critic: CNN is a critic network, defaults to False
     :type critic: bool, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
-    def __init__(self, input_shape: List[int], channel_size: List[int], kernal_size: List[int], stride_size: List[int],
-                 hidden_size: List[int], num_actions: int, num_atoms=51, mlp_activation='relu',
-                 cnn_activation='relu', layer_norm=False, stored_values=None, rainbow=False, critic=False, device='cpu'):
+
+    def __init__(
+            self,
+            input_shape: List[int],
+            channel_size: List[int],
+            kernal_size: List[int],
+            stride_size: List[int],
+            hidden_size: List[int],
+            num_actions: int,
+            num_atoms=51,
+            mlp_activation='relu',
+            cnn_activation='relu',
+            layer_norm=False,
+            stored_values=None,
+            rainbow=False,
+            critic=False,
+            device='cpu'):
 
         super(EvolvableCNN, self).__init__()
 
         self.input_shape = input_shape
         self.channel_size = channel_size
         self.kernal_size = kernal_size
         self.stride_size = stride_size
@@ -139,111 +159,150 @@
         self.critic = critic
         self.device = device
 
         self.net = self.create_nets()
         self.feature_net, self.value_net, self.advantage_net = self.create_nets()
 
         if stored_values is not None:
-            self.inject_parameters(pvec=stored_values, without_layer_norm=False)
+            self.inject_parameters(
+                pvec=stored_values, without_layer_norm=False)
 
     def get_activation(self, activation_names):
         """Returns activation function for corresponding activation name.
 
         :param activation_names: Activation function name
-        :type activation_names: str        
+        :type activation_names: str
         """
-        activation_functions = {'tanh': nn.Tanh, 'gelu': nn.GELU, 'relu': nn.ReLU, 'elu': nn.ELU,
-                                'softsign': nn.Softsign, 'sigmoid': nn.Sigmoid, 'softplus': nn.Softplus,
-                                'lrelu': nn.LeakyReLU, 'prelu': nn.PReLU, }
+        activation_functions = {
+            'tanh': nn.Tanh,
+            'gelu': nn.GELU,
+            'relu': nn.ReLU,
+            'elu': nn.ELU,
+            'softsign': nn.Softsign,
+            'sigmoid': nn.Sigmoid,
+            'softplus': nn.Softplus,
+            'lrelu': nn.LeakyReLU,
+            'prelu': nn.PReLU}
         return activation_functions[activation_names]()
 
     def create_mlp(self, input_size, output_size, hidden_size, name):
-        """Creates and returns multi-layer perceptron.        
+        """Creates and returns multi-layer perceptron.
         """
         net_dict = OrderedDict()
-        net_dict[f"{name}_linear_layer_0"] = NoisyLinear(input_size, hidden_size[0])
+        net_dict[f"{name}_linear_layer_0"] = NoisyLinear(
+            input_size, hidden_size[0])
         if self.layer_norm:
             net_dict[f"{name}_layer_norm_0"] = nn.LayerNorm(hidden_size[0])
-        net_dict[f"{name}_activation_0"] = self.get_activation(self.mlp_activation)
+        net_dict[f"{name}_activation_0"] = self.get_activation(
+            self.mlp_activation)
 
         if len(hidden_size) > 1:
             for l_no in range(1, len(hidden_size)):
-                net_dict[f"{name}_linear_layer_{str(l_no)}"] = NoisyLinear(hidden_size[l_no - 1], hidden_size[l_no])
+                net_dict[f"{name}_linear_layer_{str(l_no)}"] = NoisyLinear(
+                    hidden_size[l_no - 1], hidden_size[l_no])
                 if self.layer_norm:
-                    net_dict[f"{name}_layer_norm_{str(l_no)}"] = nn.LayerNorm(hidden_size[l_no])
-                net_dict[f"{name}_activation_{str(l_no)}"] = self.get_activation(self.mlp_activation)
-        net_dict[f"{name}_linear_layer_output"] = NoisyLinear(hidden_size[-1], output_size)
+                    net_dict[f"{name}_layer_norm_{str(l_no)}"] = nn.LayerNorm(
+                        hidden_size[l_no])
+                net_dict[f"{name}_activation_{str(l_no)}"] = self.get_activation(
+                    self.mlp_activation)
+        net_dict[f"{name}_linear_layer_output"] = NoisyLinear(
+            hidden_size[-1], output_size)
         return nn.Sequential(net_dict)
 
     def create_cnn(self, input_size, channel_size, kernal_size, stride_size, name):
-        """Creates and returns convolutional neural network.        
+        """Creates and returns convolutional neural network.
         """
         net_dict = OrderedDict()
-        net_dict[f"{name}_conv_layer_0"] = nn.Conv2d(in_channels=input_size, out_channels=channel_size[0],
-                                                     kernel_size=kernal_size[0],
-                                                     stride=stride_size[0])
+        net_dict[f"{name}_conv_layer_0"] = nn.Conv2d(
+            in_channels=input_size,
+            out_channels=channel_size[0],
+            kernel_size=kernal_size[0],
+            stride=stride_size[0])
         if self.layer_norm:
             net_dict[f"{name}_layer_norm_0"] = nn.BatchNorm2d(channel_size[0])
-        net_dict[f"{name}_activation_0"] = self.get_activation(self.cnn_activation)
+        net_dict[f"{name}_activation_0"] = self.get_activation(
+            self.cnn_activation)
 
         if len(channel_size) > 1:
             for l_no in range(1, len(channel_size)):
                 net_dict[f"{name}_conv_layer_{str(l_no)}"] = nn.Conv2d(in_channels=channel_size[l_no - 1],
                                                                        out_channels=channel_size[l_no],
                                                                        kernel_size=kernal_size[l_no],
                                                                        stride=stride_size[l_no])
                 if self.layer_norm:
-                    net_dict[f"{name}_layer_norm_{str(l_no)}"] = nn.BatchNorm2d(channel_size[l_no])
-                net_dict[f"{name}_activation_{str(l_no)}"] = self.get_activation(self.cnn_activation)
+                    net_dict[f"{name}_layer_norm_{str(l_no)}"] = nn.BatchNorm2d(
+                        channel_size[l_no])
+                net_dict[f"{name}_activation_{str(l_no)}"] = self.get_activation(
+                    self.cnn_activation)
 
         return nn.Sequential(net_dict)
 
     def create_nets(self):
-        """Creates and returns neural networks.        
+        """Creates and returns neural networks.
         """
-        feature_net = self.create_cnn(self.input_shape[0], self.channel_size, self.kernal_size, self.stride_size,
-                                      name="feature")
+        feature_net = self.create_cnn(
+            self.input_shape[0],
+            self.channel_size,
+            self.kernal_size,
+            self.stride_size,
+            name="feature")
 
-        input_size = feature_net(autograd.Variable(torch.zeros(1, *self.input_shape))).view(1, -1).size(1)
+        input_size = feature_net(autograd.Variable(
+            torch.zeros(1, *self.input_shape))).view(1, -1).size(1)
 
         if self.critic:
             input_size += self.num_actions
 
         if self.rainbow:
-            value_net = self.create_mlp(input_size, output_size=self.num_atoms, hidden_size=self.hidden_size, name="value")
-            advantage_net = self.create_mlp(input_size, output_size=self.num_atoms * self.num_actions,
-                                            hidden_size=self.hidden_size,
-                                            name="advantage")
+            value_net = self.create_mlp(
+                input_size,
+                output_size=self.num_atoms,
+                hidden_size=self.hidden_size,
+                name="value")
+            advantage_net = self.create_mlp(
+                input_size,
+                output_size=self.num_atoms *
+                self.num_actions,
+                hidden_size=self.hidden_size,
+                name="advantage")
             advantage_net.to(self.device)
         else:
             if self.critic:
-                value_net = self.create_mlp(input_size, output_size=1, hidden_size=self.hidden_size, name="value")
+                value_net = self.create_mlp(
+                    input_size,
+                    output_size=1,
+                    hidden_size=self.hidden_size,
+                    name="value")
             else:
-                value_net = self.create_mlp(input_size, output_size=self.num_actions, hidden_size=self.hidden_size, name="value")
+                value_net = self.create_mlp(
+                    input_size,
+                    output_size=self.num_actions,
+                    hidden_size=self.hidden_size,
+                    name="value")
             advantage_net = None
 
         feature_net.to(self.device)
         value_net.to(self.device)
-        
+
         return feature_net, value_net, advantage_net
 
     def reset_noise(self):
         """Resets noise of value and advantage networks.
         """
-        for l in self.value_net:
-            if isinstance(l, NoisyLinear):
-                l.reset_noise()
+        for layer in self.value_net:
+            if isinstance(layer, NoisyLinear):
+                layer.reset_noise()
         if self.rainbow:
-            for l in self.advantage_net:
-                if isinstance(l, NoisyLinear):
-                    l.reset_noise()
+            for layer in self.advantage_net:
+                if isinstance(layer, NoisyLinear):
+                    layer.reset_noise()
 
     def forward(self, x, xc=None):
         """Returns output of neural network.
-        
+
         :param x: Neural network input
         :type x: torch.Tensor() or np.array
         :param xc: Actions to be evaluated by critic, defaults to None
         :type xc: torch.Tensor() or np.array, optional
         """
         if not isinstance(x, torch.Tensor):
             x = torch.FloatTensor(x)
@@ -259,114 +318,130 @@
 
         value = self.value_net(x)
 
         if self.rainbow:
             advantage = self.advantage_net(x)
 
             value = value.view(batch_size, 1, self.num_atoms)
-            advantage = advantage.view(batch_size, self.num_actions, self.num_atoms)
+            advantage = advantage.view(
+                batch_size, self.num_actions, self.num_atoms)
 
             x = value + advantage - advantage.mean(1, keepdim=True)
-            x = F.softmax(x.view(-1, self.num_atoms), dim=-1).view(-1, self.num_actions, self.num_atoms)
+            x = F.softmax(x.view(-1, self.num_atoms), dim=-
+                          1).view(-1, self.num_actions, self.num_atoms)
 
         else:
             x = F.softmax(value, dim=-1)
 
         return x
 
     def get_model_dict(self):
         """Returns dictionary with model information and weights.
         """
         model_dict = self.init_dict
-        model_dict.update({'stored_values': self.extract_parameters(without_layer_norm=False)})
+        model_dict.update(
+            {'stored_values': self.extract_parameters(without_layer_norm=False)})
         return model_dict
 
     def count_parameters(self, without_layer_norm=False):
         """Returns number of parameters in neural network.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 count += param.data.cpu().numpy().flatten().shape[0]
         return count
 
     def extract_grad(self, without_layer_norm=False):
         """Returns current pytorch gradient in same order as genome's flattened parameter vector.
-        
+
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.grad.data.cpu().numpy().flatten().shape[0]
                 pvec[count:count + sz] = param.grad.data.cpu().numpy().flatten()
                 count += sz
         return pvec.copy()
 
     def extract_parameters(self, without_layer_norm=False):
         """Returns current flattened neural network weights.
-        
+
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.data.cpu().detach().numpy().flatten().shape[0]
                 pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
                 count += sz
         return copy.deepcopy(pvec)
 
     def inject_parameters(self, pvec, without_layer_norm=False):
         """Injects a flat vector of neural network parameters into the model's current neural network weights.
 
         :param pvec: Network weights
         :type pvec: np.array()
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         count = 0
 
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.data.cpu().numpy().flatten().shape[0]
                 raw = pvec[count:count + sz]
                 reshaped = raw.reshape(param.data.cpu().numpy().shape)
-                param.data = torch.from_numpy(copy.deepcopy(reshaped)).type(torch.FloatTensor)
+                param.data = torch.from_numpy(
+                    copy.deepcopy(reshaped)).type(torch.FloatTensor)
                 count += sz
         return pvec
-    
+
     @property
     def short_dict(self):
         """Returns shortened version of model information in dictionary.
         """
-        short_dict = {"channel_size": self.channel_size, "kernal_size": self.kernal_size,
-                      "stride_size": self.stride_size, "hidden_size": self.hidden_size,
-                      "num_atoms": self.num_atoms,
-                      "mlp_activation": self.mlp_activation, "cnn_activation": self.cnn_activation,
-                      "layer_norm": self.layer_norm}
+        short_dict = {
+            "channel_size": self.channel_size,
+            "kernal_size": self.kernal_size,
+            "stride_size": self.stride_size,
+            "hidden_size": self.hidden_size,
+            "num_atoms": self.num_atoms,
+            "mlp_activation": self.mlp_activation,
+            "cnn_activation": self.cnn_activation,
+            "layer_norm": self.layer_norm}
         return short_dict
 
     @property
     def init_dict(self):
         """Returns model information in dictionary.
         """
-        initdict = {"input_shape": self.input_shape, "channel_size": self.channel_size, "kernal_size": self.kernal_size,
-                    "stride_size": self.stride_size, "hidden_size": self.hidden_size,
-                    "num_actions": self.num_actions, "num_atoms": self.num_atoms,
-                    "mlp_activation": self.mlp_activation, "cnn_activation": self.cnn_activation,
-                    "layer_norm": self.layer_norm, "critic": self.critic, "device": self.device}
+        initdict = {
+            "input_shape": self.input_shape,
+            "channel_size": self.channel_size,
+            "kernal_size": self.kernal_size,
+            "stride_size": self.stride_size,
+            "hidden_size": self.hidden_size,
+            "num_actions": self.num_actions,
+            "num_atoms": self.num_atoms,
+            "mlp_activation": self.mlp_activation,
+            "cnn_activation": self.cnn_activation,
+            "layer_norm": self.layer_norm,
+            "critic": self.critic,
+            "device": self.device}
         return initdict
 
     def add_mlp_layer(self):
         """Adds a hidden layer to Multi-layer Perceptron.
         """
         if len(self.hidden_size) < 3:  # HARD LIMIT
             self.hidden_size += [self.hidden_size[-1]]
@@ -400,26 +475,28 @@
     def add_cnn_layer(self):
         """Adds a hidden layer to Convolutional Neural Network.
         """
         if len(self.channel_size) < 6:  # HARD LIMIT
             self.channel_size += [self.channel_size[-1]]
             self.kernal_size += [3]
 
-            stride_size_list = [[4], [4, 2], [4, 2, 1], [2, 2, 2, 1], [2, 1, 2, 1, 2], [2, 1, 2, 1, 2, 1]]
+            stride_size_list = [[4], [4, 2], [4, 2, 1], [
+                2, 2, 2, 1], [2, 1, 2, 1, 2], [2, 1, 2, 1, 2, 1]]
             self.stride_size = stride_size_list[len(self.channel_size) - 1]
 
             self.recreate_nets()
         else:
             self.add_cnn_channel()
 
     def change_cnn_kernal(self):
         """Randomly alters convolution kernal of random CNN layer.
         """
         if len(self.channel_size) > 1:
-            hidden_layer = np.random.randint(1, min(4, len(self.channel_size)), 1)[0]
+            hidden_layer = np.random.randint(
+                1, min(4, len(self.channel_size)), 1)[0]
             self.kernal_size[hidden_layer] = np.random.choice([3, 4, 5, 7])
 
             self.recreate_nets()
         else:
             self.add_cnn_layer()
 
     def add_cnn_channel(self, hidden_layer=None, numb_new_channels=None):
@@ -445,91 +522,103 @@
 
         return {"hidden_layer": hidden_layer, "numb_new_channels": numb_new_channels}
 
     def recreate_nets(self):
         """Recreates neural networks.
         """
         new_feature_net, new_value_net, new_advantage_net = self.create_nets()
-        new_feature_net = self.preserve_parameters(old_net=self.feature_net, new_net=new_feature_net)
-        new_value_net = self.preserve_parameters(old_net=self.value_net, new_net=new_value_net)
+        new_feature_net = self.preserve_parameters(
+            old_net=self.feature_net, new_net=new_feature_net)
+        new_value_net = self.preserve_parameters(
+            old_net=self.value_net, new_net=new_value_net)
         if self.rainbow:
-            new_advantage_net = self.preserve_parameters(old_net=self.advantage_net, new_net=new_advantage_net)
+            new_advantage_net = self.preserve_parameters(
+                old_net=self.advantage_net, new_net=new_advantage_net)
         self.feature_net, self.value_net, self.advantage_net = new_feature_net, new_value_net, new_advantage_net
 
     def clone(self):
         """Returns clone of neural net with identical parameters.
         """
         clone = EvolvableCNN(**copy.deepcopy(self.init_dict))
         clone.load_state_dict(self.state_dict())
         clone.rainbow = self.rainbow
         clone.critic = self.critic
         return clone
 
     def preserve_parameters(self, old_net, new_net):
         """Returns new neural network with copied parameters from old network.
-        
+
         :param old_net: Old neural network
         :type old_net: nn.Module()
         :param new_net: New neural network
         :type new_net: nn.Module()
         """
         old_net_dict = dict(old_net.named_parameters())
 
         for key, param in new_net.named_parameters():
             if key in old_net_dict.keys():
                 if old_net_dict[key].data.size() == param.data.size():
                     param.data = old_net_dict[key].data
                 else:
-                    if not "norm" in key:
+                    if "norm" not in key:
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         if len(param.data.size()) == 1:
                             param.data[:min(old_size[0], new_size[0])] = old_net_dict[key].data[
-                                                                         :min(old_size[0], new_size[0])]
+                                :min(old_size[0], new_size[0])]
                         elif len(param.data.size()) == 2:
                             param.data[:min(old_size[0], new_size[0]), :min(old_size[1], new_size[1])] = old_net_dict[
-                                                                                                             key].data[
-                                                                                                         :min(old_size[
-                                                                                                                  0],
-                                                                                                              new_size[
-                                                                                                                  0]),
-                                                                                                         :min(old_size[
-                                                                                                                  1],
-                                                                                                              new_size[
-                                                                                                                  1])]
+                                key].data[
+                                :min(old_size[
+                                    0],
+                                    new_size[
+                                    0]),
+                                :min(old_size[
+                                    1],
+                                    new_size[
+                                    1])]
                         else:
-                            param.data[:min(old_size[0], new_size[0]), :min(old_size[1], new_size[1]),
-                            :min(old_size[2], new_size[2]),
-                            :min(old_size[3], new_size[3])] = old_net_dict[key].data[
-                                                              :min(old_size[0], new_size[0]),
-                                                              :min(old_size[1], new_size[1]),
-                                                              :min(old_size[2], new_size[2]),
-                                                              :min(old_size[3], new_size[3]),
-                                                              ]
+                            param.data[:min(old_size[0],
+                                            new_size[0]),
+                                       :min(old_size[1],
+                                            new_size[1]),
+                                       :min(old_size[2],
+                                            new_size[2]),
+                                       :min(old_size[3],
+                                            new_size[3])] = old_net_dict[key].data[:min(old_size[0],
+                                                                                        new_size[0]),
+                                                                                   :min(old_size[1],
+                                                                                        new_size[1]),
+                                                                                   :min(old_size[2],
+                                                                                        new_size[2]),
+                                                                                   :min(old_size[3],
+                                                                                        new_size[3]),
+                                                                                   ]
 
         return new_net
 
     def shrink_preserve_parameters(self, old_net, new_net):
         """Returns shrunk new neural network with copied parameters from old network.
-        
+
         :param old_net: Old neural network
         :type old_net: nn.Module()
         :param new_net: New neural network
         :type new_net: nn.Module()
         """
         old_net_dict = dict(old_net.named_parameters())
 
         for key, param in new_net.named_parameters():
             if key in old_net_dict.keys():
                 if old_net_dict[key].data.size() == param.data.size():
                     param.data = old_net_dict[key].data
                 else:
-                    if not "norm" in key:
+                    if "norm" not in key:
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         min_0 = min(old_size[0], new_size[0])
                         if len(param.data.size()) == 1:
                             param.data[:min_0] = old_net_dict[key].data[:min_0]
                         else:
                             min_1 = min(old_size[1], new_size[1])
-                            param.data[:min_0, :min_1] = old_net_dict[key].data[:min_0, :min_1]
-        return new_net
+                            param.data[:min_0,
+                                       :min_1] = old_net_dict[key].data[:min_0, :min_1]
+        return new_net
```

### Comparing `agilerl-0.1.4/agilerl/networks/evolvable_mlp.py` & `agilerl-0.1.5/agilerl/networks/evolvable_mlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from collections import OrderedDict
 from typing import List
 
 import numpy as np
 import torch
 import torch.nn as nn
 
+
 class EvolvableMLP(nn.Module):
     """The Evolvable Multi-layer Perceptron class.
-    
+
     :param num_inputs: Input layer dimension
     :type num_inputs: int
     :param num_outputs: Output layer dimension
     :type num_outputs: int
     :param hidden_size: Hidden layer(s) size
     :type hidden_size: List[int]
     :param activation: Activation layer, defaults to 'relu'
@@ -24,195 +25,230 @@
     :param output_vanish: Vanish output by multiplying by 0.1, defaults to True
     :type output_vanish: bool, optional
     :param stored_values: Stored network weights, defaults to None
     :type stored_values: numpy.array(), optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
-    def __init__(self, num_inputs: int, num_outputs: int, hidden_size: List[int], activation='relu',
-                 output_activation=None, layer_norm=False, output_vanish=True, stored_values=None, device='cpu'):
+
+    def __init__(
+            self,
+            num_inputs: int,
+            num_outputs: int,
+            hidden_size: List[int],
+            activation='relu',
+            output_activation=None,
+            layer_norm=False,
+            output_vanish=True,
+            stored_values=None,
+            device='cpu'):
         super(EvolvableMLP, self).__init__()
 
         self.num_inputs = num_inputs
         self.num_outputs = num_outputs
         self.activation = activation
         self.output_activation = output_activation
         self.layer_norm = layer_norm
         self.output_vanish = output_vanish
         self.hidden_size = hidden_size
         self.device = device
 
         self.net = self.create_net()
 
         if stored_values is not None:
-            self.inject_parameters(pvec=stored_values, without_layer_norm=False)
+            self.inject_parameters(
+                pvec=stored_values, without_layer_norm=False)
 
     def get_activation(self, activation_names):
         """Returns activation function for corresponding activation name.
 
         :param activation_names: Activation function name
-        :type activation_names: str        
+        :type activation_names: str
         """
-        activation_functions = {'tanh': nn.Tanh, 'linear': nn.Identity, 'relu': nn.ReLU, 'elu': nn.ELU,
-                                'softsign': nn.Softsign, 'sigmoid': nn.Sigmoid, 'softplus': nn.Softplus,
-                                'lrelu': nn.LeakyReLU, 'prelu': nn.PReLU, }
+        activation_functions = {
+            'tanh': nn.Tanh,
+            'linear': nn.Identity,
+            'relu': nn.ReLU,
+            'elu': nn.ELU,
+            'softsign': nn.Softsign,
+            'sigmoid': nn.Sigmoid,
+            'softplus': nn.Softplus,
+            'lrelu': nn.LeakyReLU,
+            'prelu': nn.PReLU,
+            'gelu': nn.GELU}
 
         return activation_functions[activation_names]()
 
     def create_net(self):
-        """Creates and returns neural network.        
+        """Creates and returns neural network.
         """
         net_dict = OrderedDict()
 
-        net_dict["linear_layer_0"] = nn.Linear(self.num_inputs, self.hidden_size[0])
+        net_dict["linear_layer_0"] = nn.Linear(
+            self.num_inputs, self.hidden_size[0])
         if self.layer_norm:
             net_dict["layer_norm_0"] = nn.LayerNorm(self.hidden_size[0])
         net_dict["activation_0"] = self.get_activation(self.activation)
 
         if len(self.hidden_size) > 1:
             for l_no in range(1, len(self.hidden_size)):
-                net_dict[f"linear_layer_{str(l_no)}"] = nn.Linear(self.hidden_size[l_no - 1], self.hidden_size[l_no])
+                net_dict[f"linear_layer_{str(l_no)}"] = nn.Linear(
+                    self.hidden_size[l_no - 1], self.hidden_size[l_no])
                 if self.layer_norm:
-                    net_dict[f"layer_norm_{str(l_no)}"] = nn.LayerNorm(self.hidden_size[l_no])
-                net_dict[f"activation_{str(l_no)}"] = self.get_activation(self.activation)
+                    net_dict[f"layer_norm_{str(l_no)}"] = nn.LayerNorm(
+                        self.hidden_size[l_no])
+                net_dict[f"activation_{str(l_no)}"] = self.get_activation(
+                    self.activation)
 
         output_layer = nn.Linear(self.hidden_size[-1], self.num_outputs)
 
         if self.output_vanish:
             output_layer.weight.data.mul_(0.1)
             output_layer.bias.data.mul_(0.1)
 
-        net_dict[f"linear_layer_output"] = output_layer
+        net_dict["linear_layer_output"] = output_layer
         if self.output_activation is not None:
-            net_dict[f"activation_output"] = self.get_activation(self.output_activation)
+            net_dict["activation_output"] = self.get_activation(
+                self.output_activation)
 
         return nn.Sequential(net_dict)
 
     def forward(self, x):
         """Returns output of neural network.
-        
+
         :param x: Neural network input
         :type x: torch.Tensor() or np.array
         """
         if not isinstance(x, torch.Tensor):
             x = torch.FloatTensor(np.array(x)).to(self.device)
 
         for value in self.net:
             x = value(x)
         return x
 
     def get_model_dict(self):
         """Returns dictionary with model information and weights.
         """
         model_dict = self.init_dict
-        model_dict.update({'stored_values': self.extract_parameters(without_layer_norm=False)})
+        model_dict.update(
+            {'stored_values': self.extract_parameters(without_layer_norm=False)})
         return model_dict
 
     def count_parameters(self, without_layer_norm=False):
         """Returns number of parameters in neural network.
 
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 count += param.data.cpu().numpy().flatten().shape[0]
         return count
 
     def extract_grad(self, without_layer_norm=False):
         """Returns current pytorch gradient in same order as genome's flattened parameter vector.
-        
+
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.grad.data.cpu().numpy().flatten().shape[0]
                 pvec[count:count + sz] = param.grad.data.cpu().numpy().flatten()
                 count += sz
         return pvec.copy()
 
     def extract_parameters(self, without_layer_norm=False):
         """Returns current flattened neural network weights.
-        
+
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         tot_size = self.count_parameters(without_layer_norm)
         pvec = np.zeros(tot_size, np.float32)
         count = 0
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.data.cpu().detach().numpy().flatten().shape[0]
                 pvec[count:count + sz] = param.data.cpu().detach().numpy().flatten()
                 count += sz
         return copy.deepcopy(pvec)
 
     def inject_parameters(self, pvec, without_layer_norm=False):
         """Injects a flat vector of neural network parameters into the model's current neural network weights.
 
         :param pvec: Network weights
         :type pvec: np.array()
         :param without_layer_norm: Exclude normalization layers, defaults to False
-        :type without_layer_norm: bool
+        :type without_layer_norm: bool, optional
         """
         count = 0
 
         for name, param in self.named_parameters():
-            if not without_layer_norm or not 'layer_norm' in name:
+            if not without_layer_norm or 'layer_norm' not in name:
                 sz = param.data.cpu().numpy().flatten().shape[0]
                 raw = pvec[count:count + sz]
                 reshaped = raw.reshape(param.data.cpu().numpy().shape)
-                param.data = torch.from_numpy(copy.deepcopy(reshaped)).type(torch.FloatTensor)
+                param.data = torch.from_numpy(
+                    copy.deepcopy(reshaped)).type(torch.FloatTensor)
                 count += sz
         return pvec
 
     @property
     def init_dict(self):
         """Returns model information in dictionary.
         """
-        init_dict = {"num_inputs": self.num_inputs, "num_outputs": self.num_outputs, "hidden_size": self.hidden_size,
-                     "activation": self.activation, "output_activation": self.output_activation,
-                     "layer_norm": self.layer_norm}
+        init_dict = {
+            "num_inputs": self.num_inputs,
+            "num_outputs": self.num_outputs,
+            "hidden_size": self.hidden_size,
+            "activation": self.activation,
+            "output_activation": self.output_activation,
+            "layer_norm": self.layer_norm,
+            "device": self.device}
         return init_dict
 
     @property
     def short_dict(self):
         """Returns shortened version of model information in dictionary.
         """
-        short_dict = {"hidden_size": self.hidden_size,
-                      "activation": self.activation, "output_activation": self.output_activation,
-                      "layer_norm": self.layer_norm}
+        short_dict = {
+            "hidden_size": self.hidden_size,
+            "activation": self.activation,
+            "output_activation": self.output_activation,
+            "layer_norm": self.layer_norm}
         return short_dict
 
     def add_layer(self):
         """Adds a hidden layer to neural network.
         """
         # add layer to hyper params
         if len(self.hidden_size) < 3:  # HARD LIMIT
             self.hidden_size += [self.hidden_size[-1]]
 
             # copy old params to new net
             new_net = self.create_net()
-            new_net = self.preserve_parameters(old_net=self.net, new_net=new_net)
+            new_net = self.preserve_parameters(
+                old_net=self.net, new_net=new_net)
             self.net = new_net
         else:
             self.add_node()
 
     def remove_layer(self):
         """Removes a hidden layer from neural network.
         """
         if len(self.hidden_size) > 1:  # HARD LIMIT
             self.hidden_size = self.hidden_size[:1]
             new_net = self.create_net()
-            new_net = self.shrink_preserve_parameters(old_net=self.net, new_net=new_net)
+            new_net = self.shrink_preserve_parameters(
+                old_net=self.net, new_net=new_net)
             self.net = new_net
         else:
             self.add_node()
 
     def add_node(self, hidden_layer=None, numb_new_nodes=None):
         """Adds nodes to hidden layer of neural network.
 
@@ -227,15 +263,16 @@
             hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
         if numb_new_nodes is None:
             numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
 
         if self.hidden_size[hidden_layer] + numb_new_nodes <= 500:  # HARD LIMIT
             self.hidden_size[hidden_layer] += numb_new_nodes
             new_net = self.create_net()
-            new_net = self.preserve_parameters(old_net=self.net, new_net=new_net)
+            new_net = self.preserve_parameters(
+                old_net=self.net, new_net=new_net)
 
             self.net = new_net
 
         return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
 
     def remove_node(self, hidden_layer=None, numb_new_nodes=None):
         """Removes nodes from hidden layer of neural network.
@@ -249,82 +286,85 @@
             hidden_layer = np.random.randint(0, len(self.hidden_size), 1)[0]
         else:
             hidden_layer = min(hidden_layer, len(self.hidden_size) - 1)
         if numb_new_nodes is None:
             numb_new_nodes = np.random.choice([16, 32, 64], 1)[0]
 
         if self.hidden_size[hidden_layer] - numb_new_nodes > 64:  # HARD LIMIT
-            self.hidden_size[hidden_layer] = self.hidden_size[hidden_layer] - numb_new_nodes
+            self.hidden_size[hidden_layer] = self.hidden_size[hidden_layer] - \
+                numb_new_nodes
             new_net = self.create_net()
-            new_net = self.shrink_preserve_parameters(old_net=self.net, new_net=new_net)
+            new_net = self.shrink_preserve_parameters(
+                old_net=self.net, new_net=new_net)
 
             self.net = new_net
 
         return {"hidden_layer": hidden_layer, "numb_new_nodes": numb_new_nodes}
 
     def clone(self):
         """Returns clone of neural net with identical parameters.
         """
         clone = EvolvableMLP(**copy.deepcopy(self.init_dict))
         clone.load_state_dict(self.state_dict())
         return clone
 
     def preserve_parameters(self, old_net, new_net):
         """Returns new neural network with copied parameters from old network.
-        
+
         :param old_net: Old neural network
         :type old_net: nn.Module()
         :param new_net: New neural network
         :type new_net: nn.Module()
         """
         old_net_dict = dict(old_net.named_parameters())
 
         for key, param in new_net.named_parameters():
             if key in old_net_dict.keys():
                 if old_net_dict[key].data.size() == param.data.size():
                     param.data = old_net_dict[key].data
                 else:
-                    if not "norm" in key:
+                    if "norm" not in key:
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         if len(param.data.size()) == 1:
                             param.data[:min(old_size[0], new_size[0])] = old_net_dict[key].data[
-                                                                         :min(old_size[0], new_size[0])]
+                                :min(old_size[0], new_size[0])]
                         else:
                             param.data[:min(old_size[0], new_size[0]), :min(old_size[1], new_size[1])] = old_net_dict[
-                                                                                                             key].data[
-                                                                                                         :min(old_size[
-                                                                                                                  0],
-                                                                                                              new_size[
-                                                                                                                  0]),
-                                                                                                         :min(old_size[
-                                                                                                                  1],
-                                                                                                              new_size[
-                                                                                                                  1])]
+                                key].data[
+                                :min(old_size[
+                                    0],
+                                    new_size[
+                                    0]),
+                                :min(old_size[
+                                    1],
+                                    new_size[
+                                    1])]
 
         return new_net
 
     def shrink_preserve_parameters(self, old_net, new_net):
         """Returns shrunk new neural network with copied parameters from old network.
-        
+
         :param old_net: Old neural network
         :type old_net: nn.Module()
         :param new_net: New neural network
         :type new_net: nn.Module()
         """
         old_net_dict = dict(old_net.named_parameters())
 
         for key, param in new_net.named_parameters():
             if key in old_net_dict.keys():
                 if old_net_dict[key].data.size() == param.data.size():
                     param.data = old_net_dict[key].data
                 else:
-                    if not "norm" in key:
+                    if "norm" not in key:
                         old_size = old_net_dict[key].data.size()
                         new_size = param.data.size()
                         min_0 = min(old_size[0], new_size[0])
                         if len(param.data.size()) == 1:
                             param.data[:min_0] = old_net_dict[key].data[:min_0]
                         else:
                             min_1 = min(old_size[1], new_size[1])
-                            param.data[:min_0, :min_1] = old_net_dict[key].data[:min_0, :min_1]
+                            param.data[:min_0,
+                                       :min_1] = old_net_dict[key].data[:min_0, :min_1]
         return new_net
```

### Comparing `agilerl-0.1.4/agilerl/training/train.py` & `agilerl-0.1.5/agilerl/training/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 import numpy as np
 from tqdm import trange
 import wandb
 from datetime import datetime
 
-def train(env, env_name, algo, pop, memory, swap_channels=False, n_episodes=2000, max_steps=500, evo_epochs=5, evo_loop=1, eps_start=1.0, eps_end=0.1, eps_decay=0.995, target=200., tournament=None, mutation=None, checkpoint=None, checkpoint_path=None, wb=False, device='cpu'):
-    """The general training function. Returns trained population of agents and their fitnesses. 
+
+def train(
+        env,
+        env_name,
+        algo,
+        pop,
+        memory,
+        swap_channels=False,
+        n_episodes=2000,
+        max_steps=500,
+        evo_epochs=5,
+        evo_loop=1,
+        eps_start=1.0,
+        eps_end=0.1,
+        eps_decay=0.995,
+        target=200.,
+        tournament=None,
+        mutation=None,
+        checkpoint=None,
+        checkpoint_path=None,
+        wb=False,
+        device='cpu'):
+    """The general training function. Returns trained population of agents and their fitnesses.
 
     :param env: The environment to train in. Can be vectorized.
     :type env: Gym-style environment
     :param env_name: Environment name
     :type env_name: str
     :param algo: RL algorithm name
     :type algo: str
@@ -47,24 +68,26 @@
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
     if wb:
         wandb.init(
             # set the wandb project where this run will be logged
             project="AgileRL",
-            name="{}-EvoHPO-{}-{}".format(env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S")),
+            name="{}-EvoHPO-{}-{}".format(env_name, algo,
+                                          datetime.now().strftime("%m%d%Y%H%M%S")),
             # track hyperparameters and run metadata
             config={
-            "algo": "Evo HPO {}".format(algo),
-            "env": env_name,
+                "algo": "Evo HPO {}".format(algo),
+                "env": env_name,
             }
         )
 
-    save_path = checkpoint_path.split('.pt')[0] if checkpoint_path is not None else "{}-EvoHPO-{}-{}".format(env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S"))
-    
+    save_path = checkpoint_path.split('.pt')[0] if checkpoint_path is not None else "{}-EvoHPO-{}-{}".format(
+        env_name, algo, datetime.now().strftime("%m%d%Y%H%M%S"))
+
     epsilon = eps_start
 
     bar_format = '{l_bar}{bar:10}| {n:4}/{total_fmt} [{elapsed:>7}<{remaining:>7}, {rate_fmt}{postfix}]'
     pbar = trange(n_episodes, unit="ep", bar_format=bar_format, ascii=True)
 
     pop_fitnesses = []
     total_steps = 0
@@ -74,70 +97,88 @@
         for agent in pop:   # Loop through population
             state = env.reset()[0]  # Reset environment at start of episode
             score = 0
 
             for idx_step in range(max_steps):
                 if swap_channels:
                     state = np.moveaxis(state, [3], [1])
-                action = agent.getAction(state, epsilon)    # Get next action from agent
-                next_state, reward, done, _, _ = env.step(action)   # Act in environment
+                # Get next action from agent
+                action = agent.getAction(state, epsilon)
+                next_state, reward, done, _, _ = env.step(
+                    action)   # Act in environment
 
                 # Save experience to replay buffer
                 if swap_channels:
-                    memory.save2memoryVectEnvs(state, action, reward, np.moveaxis(next_state, [3], [1]), done)
+                    memory.save2memoryVectEnvs(
+                        state, action, reward, np.moveaxis(next_state, [3], [1]), done)
                 else:
-                    memory.save2memoryVectEnvs(state, action, reward, next_state, done)
+                    memory.save2memoryVectEnvs(
+                        state, action, reward, next_state, done)
 
                 # Learn according to learning frequency
-                if memory.counter % agent.learn_step == 0 and len(memory) >= agent.batch_size:
-                    experiences = memory.sample(agent.batch_size)   # Sample replay buffer
-                    agent.learn(experiences)    # Learn according to agent's RL algorithm
+                if memory.counter % agent.learn_step == 0 and len(
+                        memory) >= agent.batch_size:
+                    experiences = memory.sample(
+                        agent.batch_size)   # Sample replay buffer
+                    # Learn according to agent's RL algorithm
+                    agent.learn(experiences)
 
                 state = next_state
                 score += reward
-            
+
             agent.scores.append(score)
-            
+
             agent.steps[-1] += max_steps
             total_steps += max_steps
 
-        epsilon = max(eps_end, epsilon*eps_decay)   # Update epsilon for exploration
+        # Update epsilon for exploration
+        epsilon = max(eps_end, epsilon * eps_decay)
 
         # Now evolve if necessary
-        if (idx_epi+1) % evo_epochs == 0:
-            
+        if (idx_epi + 1) % evo_epochs == 0:
+
             # Evaluate population
-            fitnesses = [agent.test(env, swap_channels=swap_channels, max_steps=max_steps, loop=evo_loop) for agent in pop]
+            fitnesses = [
+                agent.test(
+                    env,
+                    swap_channels=swap_channels,
+                    max_steps=max_steps,
+                    loop=evo_loop) for agent in pop]
             pop_fitnesses.append(fitnesses)
 
-            mean_scores = np.mean([agent.scores[-20:] for agent in pop], axis=1)
+            mean_scores = np.mean([agent.scores[-20:]
+                                  for agent in pop], axis=1)
 
             if wb:
-                wandb.log({"global_step": total_steps, "eval/mean_score": np.mean(mean_scores), "eval/mean_reward": np.mean(fitnesses), "eval/best_fitness": np.max(fitnesses)})
-            
+                wandb.log({"global_step": total_steps,
+                           "eval/mean_score": np.mean(mean_scores),
+                           "eval/mean_reward": np.mean(fitnesses),
+                           "eval/best_fitness": np.max(fitnesses)})
+
             # Update step counter
             for agent in pop:
                 agent.steps.append(agent.steps[-1])
 
             pbar.set_postfix_str(f'Fitness: {["%.2f"%fitness for fitness in fitnesses]}, 100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}, 100 score avgs: {["%.2f"%np.mean(agent.scores[-100:]) for agent in pop]}, agents: {[agent.index for agent in pop]}, steps: {[agent.steps[-1] for agent in pop]}, mutations: {[agent.mut for agent in pop]}')
             pbar.update(0)
 
             # Early stop if consistently reaches target
-            if np.all(np.greater([np.mean(agent.fitness[-100:]) for agent in pop], target)) and idx_epi >= 100:
+            if np.all(np.greater([np.mean(agent.fitness[-100:])
+                      for agent in pop], target)) and idx_epi >= 100:
                 if wb:
                     wandb.finish()
                 return pop, pop_fitnesses
 
             if tournament and mutation is not None:
                 # Tournament selection and population mutation
                 elite, pop = tournament.select(pop)
                 pop = mutation.mutation(pop)
 
         # Save model checkpoint
         if checkpoint is not None:
-            if (idx_epi+1) % checkpoint == 0:
+            if (idx_epi + 1) % checkpoint == 0:
                 for i, agent in enumerate(pop):
                     agent.saveCheckpoint(f'{save_path}_{i}_{idx_epi+1}.pt')
 
     if wb:
         wandb.finish()
     return pop, pop_fitnesses
```

### Comparing `agilerl-0.1.4/agilerl/utils.py` & `agilerl-0.1.5/agilerl/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import gymnasium as gym
 import numpy as np
 import matplotlib.pyplot as plt
 from agilerl.algorithms.dqn import DQN
 from agilerl.algorithms.ddpg import DDPG
 
+
 def makeVectEnvs(env_name, num_envs=1):
     """Returns async-vectorized gym environments.
 
     :param env_name: Gym environment name
     :type env_name: str
     :param num_ens: Number of vectorized environments, defaults to 1
     :type num_envs: int, optional
     """
-    return gym.vector.AsyncVectorEnv([lambda: gym.make(env_name) for i in range(num_envs)])
- 
+    return gym.vector.AsyncVectorEnv(
+        [lambda: gym.make(env_name) for i in range(num_envs)])
+
 
-def initialPopulation(algo, state_dim, action_dim, one_hot, net_config, INIT_HP, population_size=1, device='cpu'):
+def initialPopulation(algo, state_dim, action_dim, one_hot,
+                      net_config, INIT_HP, population_size=1, device='cpu'):
     """Returns population of identical agents.
-    
+
     :param algo: RL algorithm
     :type algo: str
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
     :param one_hot: One-hot encoding
@@ -34,56 +37,59 @@
     :type device: str, optional
     """
     population = []
 
     if algo == 'DQN':
         for idx in range(population_size):
             agent = DQN(
-                state_dim = state_dim,
-                action_dim = action_dim,
-                one_hot = one_hot,
-                index = idx,
-                net_config = net_config,
-                batch_size = INIT_HP['BATCH_SIZE'],
-                lr = INIT_HP['LR'],
-                learn_step = INIT_HP['LEARN_STEP'],
-                gamma = INIT_HP['GAMMA'],
-                tau = INIT_HP['TAU'],
+                state_dim=state_dim,
+                action_dim=action_dim,
+                one_hot=one_hot,
+                index=idx,
+                net_config=net_config,
+                batch_size=INIT_HP['BATCH_SIZE'],
+                lr=INIT_HP['LR'],
+                learn_step=INIT_HP['LEARN_STEP'],
+                gamma=INIT_HP['GAMMA'],
+                tau=INIT_HP['TAU'],
                 device=device
-                )
+            )
             population.append(agent)
 
     elif algo == 'DDPG':
         for idx in range(population_size):
             agent = DDPG(
-                state_dim = state_dim,
-                action_dim = action_dim,
-                one_hot = one_hot,
-                index = idx,
-                net_config = net_config,
-                batch_size = INIT_HP['BATCH_SIZE'],
-                lr = INIT_HP['LR'],
-                learn_step = INIT_HP['LEARN_STEP'],
-                gamma = INIT_HP['GAMMA'],
-                tau = INIT_HP['TAU'],
-                policy_freq = INIT_HP['POLICY_FREQ'],
+                state_dim=state_dim,
+                action_dim=action_dim,
+                one_hot=one_hot,
+                index=idx,
+                net_config=net_config,
+                batch_size=INIT_HP['BATCH_SIZE'],
+                lr=INIT_HP['LR'],
+                learn_step=INIT_HP['LEARN_STEP'],
+                gamma=INIT_HP['GAMMA'],
+                tau=INIT_HP['TAU'],
+                policy_freq=INIT_HP['POLICY_FREQ'],
                 device=device
-                )
+            )
             population.append(agent)
 
     return population
 
+
 def printHyperparams(pop):
     """Prints current hyperparameters of agents in a population and their fitnesses.
 
     :param pop: Population of agents
     :type pop: List[object]
     """
     for agent in pop:
-        print('Agent ID: {}    Mean 100 fitness: {:.2f}    lr: {}    Batch Size: {}'.format(agent.index, np.mean(agent.fitness[-100:]), agent.lr, agent.batch_size))
+        print('Agent ID: {}    Mean 100 fitness: {:.2f}    lr: {}    Batch Size: {}'.format(
+            agent.index, np.mean(agent.fitness[-100:]), agent.lr, agent.batch_size))
+
 
 def plotPopulationScore(pop):
     """Plots the fitness scores of agents in a population.
 
     :param pop: Population of agents
     :type pop: List[object]
     """
@@ -91,8 +97,8 @@
     for agent in pop:
         scores = agent.fitness
         steps = agent.steps[:-1]
         plt.plot(steps, scores)
     plt.title("Score History - Mutations")
     plt.xlabel("Steps")
     plt.ylim(bottom=-400)
-    plt.show()
+    plt.show()
```

### Comparing `agilerl-0.1.4/LICENSE` & `agilerl-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.4/pyproject.toml` & `agilerl-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agilerl"
-version = "0.1.4"
+version = "0.1.5"
 description = "AgileRL is a deep reinforcement learning library focused on improving RL development through RLOps."
 authors = ["Nick Ustaran-Anderegg <dev@agilerl.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agilerl-0.1.4/README.md` & `agilerl-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,32 @@
 
 This is a Deep Reinforcement Learning library focused on improving development by introducing RLOps - MLOps for reinforcement learning.
   
 This library is initially focused on reducing the time taken for training models and hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for reinforcement learning.<br>
 Evolutionary HPO has been shown to drastically reduce overall training times by automatically converging on optimal hyperparameters, without requiring numerous training runs.<br>
 We are constantly adding more algorithms, with a view to add hierarchical and multi-agent algorithms soon.
 
-### Benchmarks
+<p align="center">
+  <img src=https://user-images.githubusercontent.com/47857277/236407686-21363eb3-ffcf-419f-b019-0be4ddf1ed4a.gif height="250">
+</p>
+<p align="center">AgileRL offers 10x faster hyperparameter optimization than SOTA.<br> Global steps is the sum of every step taken by any agent in the environment, including across an entire population, during the entire hyperparameter optimization process.</p>
+
+## Table of Contents
+  * [Benchmarks](#benchmarks)
+  * [Get Started](#get-started)
+  * [Algorithms implemented](#algorithms-implemented-more-coming-soon)
+  * [Train an agent on a Gym environment](#train-an-agent-on-a-gym-environment)
+    + [Custom Training Loop](#custom-training-loop)
+  * [Train an agent on a language environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf)
+
+## Benchmarks
 
 Reinforcement learning algorithms and libraries are usually benchmarked once the optimal hyperparameters for training are known, but it often takes hundreds or thousands of experiments to discover these. This is unrealistic and does not reflect the true, total time taken for training. What if we could remove the need to conduct all these prior experiments?
 
-In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible.
+In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible. Global steps is the sum of every step taken by any agent in the environment, including across an entire population.
 
 <p align="center">
   <img src=https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-4655-ab32-90d659a71c69.png height="500">
 </p>
 <p align="center">AgileRL offers an order of magnitude speed up in hyperparameter optimization vs popular reinforcement learning training frameworks combined with Optuna. Remove the need for multiple training runs and save yourself hours.</p>
 
 ## Get Started
@@ -36,24 +49,27 @@
 pip install agilerl
 ```
 Or install in development mode: (Recommended due to nascent nature of this library)
 ```bash
 git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt
 ```
+If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>. 
+
 Demo:
 ```bash
 python demo.py
 ```
 
 ## Algorithms implemented (more coming soon!)
   * DQN
   * DDPG
+  * ILQL
 
-## Train an agent
+## Train an agent on a Gym environment
 Before starting training, there are some meta-hyperparameters and settings that must be set. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
 ```python
 INIT_HP = {
     'ENV_NAME': 'LunarLander-v2',   # Gym environment name
     'ALGO': 'DQN',                  # Algorithm
     'CHANNELS_LAST': False,         # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
     'BATCH_SIZE': 256,              # Batch size
@@ -280,8 +296,27 @@
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
         # Tournament selection and population mutation
         elite, pop = tournament.select(pop)
         pop = mutations.mutation(pop)
 ```
 
+## Train an agent on a language environment (RLHF)
+We implement RLHF on Wordle, and use <a href="https://arxiv.org/pdf/2206.11871.pdf">ILQL</a> to finetune our model. To create your own language environment, 
+see https://github.com/Sea-Snell/Implicit-Language-Q-Learning.
+The <code>EvolvableGPT</code> class allows us to combine LLMs and transformer architectures with evolvable HPO, which can massively reduce the time taken to finetune 
+these expensive models. Due to the vast number of parameters and settings involved in training a Large Language Model (LLM) on human feedback, these are defined in 
+<code>configs</code>. 
+
+In order to finetune a model with RLHF, we need a trained model as a starting point. We can use behavioural cloning (BC, supervised learning) to build this first version of 
+the model. To train your own model from scratch:
+```bash
+python run_bc_lm.py
+```
+If you want to use pretrained model weights, these can be defined in <code>configs/wordle/train_bc.yaml</code> in <code>model: load:</code>.
+
+Similarly, to then run ILQL and perform RLHF on the BC model:
+```bash
+python run_ilql.py
+```
+
 View <a href="https://agilerl.readthedocs.io/en/latest/">documentation</a>.
```

#### html2text {}

```diff
@@ -17,35 +17,49 @@
 initially focused on reducing the time taken for training models and
 hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for
 reinforcement learning.
 Evolutionary HPO has been shown to drastically reduce overall training times by
 automatically converging on optimal hyperparameters, without requiring numerous
 training runs.
 We are constantly adding more algorithms, with a view to add hierarchical and
-multi-agent algorithms soon. ### Benchmarks Reinforcement learning algorithms
-and libraries are usually benchmarked once the optimal hyperparameters for
-training are known, but it often takes hundreds or thousands of experiments to
-discover these. This is unrealistic and does not reflect the true, total time
-taken for training. What if we could remove the need to conduct all these prior
-experiments? In the charts below, a single AgileRL run, which automatically
-tunes hyperparameters, is benchmarked against Optuna's multiple training runs
-traditionally required for hyperparameter optimization, demonstrating the real
-time savings possible.
+multi-agent algorithms soon.
+ [https://user-images.githubusercontent.com/47857277/236407686-21363eb3-ffcf-
+                          419f-b019-0be4ddf1ed4a.gif]
+       AgileRL offers 10x faster hyperparameter optimization than SOTA.
+ Global steps is the sum of every step taken by any agent in the environment,
+    including across an entire population, during the entire hyperparameter
+                             optimization process.
+## Table of Contents * [Benchmarks](#benchmarks) * [Get Started](#get-started)
+* [Algorithms implemented](#algorithms-implemented-more-coming-soon) * [Train
+an agent on a Gym environment](#train-an-agent-on-a-gym-environment) + [Custom
+Training Loop](#custom-training-loop) * [Train an agent on a language
+environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) ##
+Benchmarks Reinforcement learning algorithms and libraries are usually
+benchmarked once the optimal hyperparameters for training are known, but it
+often takes hundreds or thousands of experiments to discover these. This is
+unrealistic and does not reflect the true, total time taken for training. What
+if we could remove the need to conduct all these prior experiments? In the
+charts below, a single AgileRL run, which automatically tunes hyperparameters,
+is benchmarked against Optuna's multiple training runs traditionally required
+for hyperparameter optimization, demonstrating the real time savings possible.
+Global steps is the sum of every step taken by any agent in the environment,
+including across an entire population.
  [https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-
                           4655-ab32-90d659a71c69.png]
 AgileRL offers an order of magnitude speed up in hyperparameter optimization vs
 popular reinforcement learning training frameworks combined with Optuna. Remove
          the need for multiple training runs and save yourself hours.
 ## Get Started Install as a package with pip: ```bash pip install agilerl ```
 Or install in development mode: (Recommended due to nascent nature of this
 library) ```bash git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
-pip install -r requirements.txt ``` Demo: ```bash python demo.py ``` ##
-Algorithms implemented (more coming soon!) * DQN * DDPG ## Train an agent
-Before starting training, there are some meta-hyperparameters and settings that
-must be set. These are defined in INIT_HP, for general parameters, and
+pip install -r requirements.txt ``` If using ILQL on Wordle, download and unzip
+data.zip here. Demo: ```bash python demo.py ``` ## Algorithms implemented (more
+coming soon!) * DQN * DDPG * ILQL ## Train an agent on a Gym environment Before
+starting training, there are some meta-hyperparameters and settings that must
+be set. These are defined in INIT_HP, for general parameters, and
 MUTATION_PARAMS, which define the evolutionary probabilities, and NET_CONFIG,
 which defines the network architecture. For example: ```python INIT_HP =
 { 'ENV_NAME': 'LunarLander-v2', # Gym environment name 'ALGO': 'DQN', #
 Algorithm 'CHANNELS_LAST': False, # Swap image channels dimension from last to
 first [H, W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
 Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
 Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
@@ -158,8 +172,22 @@
 epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration #
 Now evolve population if necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate
 population fitnesses = [agent.test(env, swap_channels=False,
 max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
 {idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
 fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
 for agent in pop]}') # Tournament selection and population mutation elite, pop
-= tournament.select(pop) pop = mutations.mutation(pop) ``` View documentation.
+= tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
+a language environment (RLHF) We implement RLHF on Wordle, and use ILQL to
+finetune our model. To create your own language environment, see https://
+github.com/Sea-Snell/Implicit-Language-Q-Learning. The EvolvableGPT class
+allows us to combine LLMs and transformer architectures with evolvable HPO,
+which can massively reduce the time taken to finetune these expensive models.
+Due to the vast number of parameters and settings involved in training a Large
+Language Model (LLM) on human feedback, these are defined in configs. In order
+to finetune a model with RLHF, we need a trained model as a starting point. We
+can use behavioural cloning (BC, supervised learning) to build this first
+version of the model. To train your own model from scratch: ```bash python
+run_bc_lm.py ``` If you want to use pretrained model weights, these can be
+defined in configs/wordle/train_bc.yaml in model: load:. Similarly, to then run
+ILQL and perform RLHF on the BC model: ```bash python run_ilql.py ``` View
+documentation.
```

### Comparing `agilerl-0.1.4/PKG-INFO` & `agilerl-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agilerl
-Version: 0.1.4
+Version: 0.1.5
 Summary: AgileRL is a deep reinforcement learning library focused on improving RL development through RLOps.
 License: Apache 2.0
 Author: Nick Ustaran-Anderegg
 Author-email: dev@agilerl.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -38,19 +38,32 @@
 
 This is a Deep Reinforcement Learning library focused on improving development by introducing RLOps - MLOps for reinforcement learning.
   
 This library is initially focused on reducing the time taken for training models and hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for reinforcement learning.<br>
 Evolutionary HPO has been shown to drastically reduce overall training times by automatically converging on optimal hyperparameters, without requiring numerous training runs.<br>
 We are constantly adding more algorithms, with a view to add hierarchical and multi-agent algorithms soon.
 
-### Benchmarks
+<p align="center">
+  <img src=https://user-images.githubusercontent.com/47857277/236407686-21363eb3-ffcf-419f-b019-0be4ddf1ed4a.gif height="250">
+</p>
+<p align="center">AgileRL offers 10x faster hyperparameter optimization than SOTA.<br> Global steps is the sum of every step taken by any agent in the environment, including across an entire population, during the entire hyperparameter optimization process.</p>
+
+## Table of Contents
+  * [Benchmarks](#benchmarks)
+  * [Get Started](#get-started)
+  * [Algorithms implemented](#algorithms-implemented-more-coming-soon)
+  * [Train an agent on a Gym environment](#train-an-agent-on-a-gym-environment)
+    + [Custom Training Loop](#custom-training-loop)
+  * [Train an agent on a language environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf)
+
+## Benchmarks
 
 Reinforcement learning algorithms and libraries are usually benchmarked once the optimal hyperparameters for training are known, but it often takes hundreds or thousands of experiments to discover these. This is unrealistic and does not reflect the true, total time taken for training. What if we could remove the need to conduct all these prior experiments?
 
-In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible.
+In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible. Global steps is the sum of every step taken by any agent in the environment, including across an entire population.
 
 <p align="center">
   <img src=https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-4655-ab32-90d659a71c69.png height="500">
 </p>
 <p align="center">AgileRL offers an order of magnitude speed up in hyperparameter optimization vs popular reinforcement learning training frameworks combined with Optuna. Remove the need for multiple training runs and save yourself hours.</p>
 
 ## Get Started
@@ -59,24 +72,27 @@
 pip install agilerl
 ```
 Or install in development mode: (Recommended due to nascent nature of this library)
 ```bash
 git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt
 ```
+If using ILQL on Wordle, download and unzip data.zip <a href="https://drive.google.com/drive/folders/13LFspsFQ-7XIlFjnsZttKf4nfVDlnmW2?usp=sharing">here</a>. 
+
 Demo:
 ```bash
 python demo.py
 ```
 
 ## Algorithms implemented (more coming soon!)
   * DQN
   * DDPG
+  * ILQL
 
-## Train an agent
+## Train an agent on a Gym environment
 Before starting training, there are some meta-hyperparameters and settings that must be set. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
 ```python
 INIT_HP = {
     'ENV_NAME': 'LunarLander-v2',   # Gym environment name
     'ALGO': 'DQN',                  # Algorithm
     'CHANNELS_LAST': False,         # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
     'BATCH_SIZE': 256,              # Batch size
@@ -303,9 +319,28 @@
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
         # Tournament selection and population mutation
         elite, pop = tournament.select(pop)
         pop = mutations.mutation(pop)
 ```
 
+## Train an agent on a language environment (RLHF)
+We implement RLHF on Wordle, and use <a href="https://arxiv.org/pdf/2206.11871.pdf">ILQL</a> to finetune our model. To create your own language environment, 
+see https://github.com/Sea-Snell/Implicit-Language-Q-Learning.
+The <code>EvolvableGPT</code> class allows us to combine LLMs and transformer architectures with evolvable HPO, which can massively reduce the time taken to finetune 
+these expensive models. Due to the vast number of parameters and settings involved in training a Large Language Model (LLM) on human feedback, these are defined in 
+<code>configs</code>. 
+
+In order to finetune a model with RLHF, we need a trained model as a starting point. We can use behavioural cloning (BC, supervised learning) to build this first version of 
+the model. To train your own model from scratch:
+```bash
+python run_bc_lm.py
+```
+If you want to use pretrained model weights, these can be defined in <code>configs/wordle/train_bc.yaml</code> in <code>model: load:</code>.
+
+Similarly, to then run ILQL and perform RLHF on the BC model:
+```bash
+python run_ilql.py
+```
+
 View <a href="https://agilerl.readthedocs.io/en/latest/">documentation</a>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agilerl Version: 0.1.4 Summary: AgileRL is a deep
+Metadata-Version: 2.1 Name: agilerl Version: 0.1.5 Summary: AgileRL is a deep
 reinforcement learning library focused on improving RL development through
 RLOps. License: Apache 2.0 Author: Nick Ustaran-Anderegg Author-email:
 dev@agilerl.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fastrand (>=1.3.0,<2.0.0)
@@ -28,35 +28,49 @@
 initially focused on reducing the time taken for training models and
 hyperparameter optimization (HPO) by pioneering evolutionary HPO techniques for
 reinforcement learning.
 Evolutionary HPO has been shown to drastically reduce overall training times by
 automatically converging on optimal hyperparameters, without requiring numerous
 training runs.
 We are constantly adding more algorithms, with a view to add hierarchical and
-multi-agent algorithms soon. ### Benchmarks Reinforcement learning algorithms
-and libraries are usually benchmarked once the optimal hyperparameters for
-training are known, but it often takes hundreds or thousands of experiments to
-discover these. This is unrealistic and does not reflect the true, total time
-taken for training. What if we could remove the need to conduct all these prior
-experiments? In the charts below, a single AgileRL run, which automatically
-tunes hyperparameters, is benchmarked against Optuna's multiple training runs
-traditionally required for hyperparameter optimization, demonstrating the real
-time savings possible.
+multi-agent algorithms soon.
+ [https://user-images.githubusercontent.com/47857277/236407686-21363eb3-ffcf-
+                          419f-b019-0be4ddf1ed4a.gif]
+       AgileRL offers 10x faster hyperparameter optimization than SOTA.
+ Global steps is the sum of every step taken by any agent in the environment,
+    including across an entire population, during the entire hyperparameter
+                             optimization process.
+## Table of Contents * [Benchmarks](#benchmarks) * [Get Started](#get-started)
+* [Algorithms implemented](#algorithms-implemented-more-coming-soon) * [Train
+an agent on a Gym environment](#train-an-agent-on-a-gym-environment) + [Custom
+Training Loop](#custom-training-loop) * [Train an agent on a language
+environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) ##
+Benchmarks Reinforcement learning algorithms and libraries are usually
+benchmarked once the optimal hyperparameters for training are known, but it
+often takes hundreds or thousands of experiments to discover these. This is
+unrealistic and does not reflect the true, total time taken for training. What
+if we could remove the need to conduct all these prior experiments? In the
+charts below, a single AgileRL run, which automatically tunes hyperparameters,
+is benchmarked against Optuna's multiple training runs traditionally required
+for hyperparameter optimization, demonstrating the real time savings possible.
+Global steps is the sum of every step taken by any agent in the environment,
+including across an entire population.
  [https://user-images.githubusercontent.com/47857277/227481592-27a9688f-7c0a-
                           4655-ab32-90d659a71c69.png]
 AgileRL offers an order of magnitude speed up in hyperparameter optimization vs
 popular reinforcement learning training frameworks combined with Optuna. Remove
          the need for multiple training runs and save yourself hours.
 ## Get Started Install as a package with pip: ```bash pip install agilerl ```
 Or install in development mode: (Recommended due to nascent nature of this
 library) ```bash git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
-pip install -r requirements.txt ``` Demo: ```bash python demo.py ``` ##
-Algorithms implemented (more coming soon!) * DQN * DDPG ## Train an agent
-Before starting training, there are some meta-hyperparameters and settings that
-must be set. These are defined in INIT_HP, for general parameters, and
+pip install -r requirements.txt ``` If using ILQL on Wordle, download and unzip
+data.zip here. Demo: ```bash python demo.py ``` ## Algorithms implemented (more
+coming soon!) * DQN * DDPG * ILQL ## Train an agent on a Gym environment Before
+starting training, there are some meta-hyperparameters and settings that must
+be set. These are defined in INIT_HP, for general parameters, and
 MUTATION_PARAMS, which define the evolutionary probabilities, and NET_CONFIG,
 which defines the network architecture. For example: ```python INIT_HP =
 { 'ENV_NAME': 'LunarLander-v2', # Gym environment name 'ALGO': 'DQN', #
 Algorithm 'CHANNELS_LAST': False, # Swap image channels dimension from last to
 first [H, W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
 Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
 Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
@@ -169,8 +183,22 @@
 epsilon = max(eps_end, epsilon*eps_decay) # Update epsilon for exploration #
 Now evolve population if necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate
 population fitnesses = [agent.test(env, swap_channels=False,
 max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
 {idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
 fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
 for agent in pop]}') # Tournament selection and population mutation elite, pop
-= tournament.select(pop) pop = mutations.mutation(pop) ``` View documentation.
+= tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
+a language environment (RLHF) We implement RLHF on Wordle, and use ILQL to
+finetune our model. To create your own language environment, see https://
+github.com/Sea-Snell/Implicit-Language-Q-Learning. The EvolvableGPT class
+allows us to combine LLMs and transformer architectures with evolvable HPO,
+which can massively reduce the time taken to finetune these expensive models.
+Due to the vast number of parameters and settings involved in training a Large
+Language Model (LLM) on human feedback, these are defined in configs. In order
+to finetune a model with RLHF, we need a trained model as a starting point. We
+can use behavioural cloning (BC, supervised learning) to build this first
+version of the model. To train your own model from scratch: ```bash python
+run_bc_lm.py ``` If you want to use pretrained model weights, these can be
+defined in configs/wordle/train_bc.yaml in model: load:. Similarly, to then run
+ILQL and perform RLHF on the BC model: ```bash python run_ilql.py ``` View
+documentation.
```

