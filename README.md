<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Roteiro de Trabalho Diário - MPPB</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .task-item input[type="checkbox"] {
            transform: scale(1.2);
            margin-right: 12px;
            accent-color: #3b82f6; /* blue-500 */
        }
        .task-item input[type="checkbox"]:checked + label {
            text-decoration: line-through;
            color: #6b7280; /* gray-500 */
        }
        .task-item {
            display: flex;
            align-items: center;
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800 p-4 sm:p-6 md:p-8">
    <div class="max-w-4xl mx-auto">
        <header class="text-center mb-8">
            <h1 class="text-3xl md:text-4xl font-bold text-gray-700">Roteiro de Trabalho Diário</h1>
            <p class="text-lg text-gray-500 mt-2">Assessor em Substituição - MPPB</p>
        </header>

        <main class="grid grid-cols-1 lg:grid-cols-2 gap-8">
            <!-- Coluna Guarabira -->
            <div class="bg-white p-6 rounded-xl shadow-md border border-gray-200">
                <div class="flex items-center justify-between mb-6">
                    <h2 class="text-2xl font-bold text-blue-700">Promotoria de Guarabira</h2>
                    <span class="bg-blue-100 text-blue-800 text-sm font-semibold px-3 py-1 rounded-full">07:00 - 10:00</span>
                </div>

                <ul class="space-y-5">
                    <!-- Urgências -->
                    <li class="p-4 bg-yellow-50 border border-yellow-200 rounded-lg">
                        <div class="task-item">
                            <input type="checkbox" id="g_urgencia_check" class="flex-shrink-0">
                            <label for="g_urgencia_check" class="font-semibold text-yellow-800">Verificar Urgências (WhatsApp)</label>
                        </div>
                        <input type="text" placeholder="Anotar urgência do dia aqui..." class="mt-2 w-full bg-white border border-gray-300 rounded-md px-3 py-2 text-sm focus:ring-blue-500 focus:border-blue-500">
                    </li>

                    <!-- Prazos -->
                    <li>
                        <div class="task-item">
                            <input type="checkbox" id="g_prazos_check">
                            <label for="g_prazos_check" class="font-semibold">Analisar Prazos (Vencidos e Vincendos)</label>
                        </div>
                        <ul class="mt-3 ml-10 space-y-2 text-sm text-gray-600">
                            <li class="task-item"><input type="checkbox" id="g_p_minha_caixa"><label for="g_p_minha_caixa">Minha Caixa</label></li>
                            <li class="task-item"><input type="checkbox" id="g_p_fabiana"><label for="g_p_fabiana">Fabiana Peixoto</label></li>
                            <li class="task-item"><input type="checkbox" id="g_p_jailson"><label for="g_p_jailson">Jailson Alves</label></li>
                            <li class="task-item"><input type="checkbox" id="g_p_anita"><label for="g_p_anita">Anita Rocha (Membra)</label></li>
                        </ul>
                    </li>

                    <!-- Prazos Judiciais -->
                    <li class="task-item">
                        <input type="checkbox" id="g_judicial_check">
                        <label for="g_judicial_check" class="font-semibold">Analisar Prazos Judiciais (resolver 1 dia antes)</label>
                    </li>
                    
                    <!-- Sem Movimento -->
                    <li class="task-item">
                        <input type="checkbox" id="g_movimento_check">
                        <label for="g_movimento_check" class="font-semibold">Verificar procedimentos sem movimento (+30 dias)</label>
                    </li>

                    <!-- Tempo extra -->
                    <li class="task-item">
                        <input type="checkbox" id="g_extra_check">
                        <label for="g_extra_check" class="font-semibold text-green-700">Se sobrar tempo: adiantar próximos vencimentos</label>
                    </li>
                </ul>
            </div>

            <!-- Coluna Picuí -->
            <div class="bg-white p-6 rounded-xl shadow-md border border-gray-200">
                <div class="flex items-center justify-between mb-6">
                    <h2 class="text-2xl font-bold text-teal-700">Promotoria de Picuí</h2>
                    <span class="bg-teal-100 text-teal-800 text-sm font-semibold px-3 py-1 rounded-full">10:30 - 13:00</span>
                </div>
                 <ul class="space-y-5">
                    <!-- Urgências -->
                    <li class="p-4 bg-yellow-50 border border-yellow-200 rounded-lg">
                        <div class="task-item">
                            <input type="checkbox" id="p_urgencia_check" class="flex-shrink-0">
                            <label for="p_urgencia_check" class="font-semibold text-yellow-800">Verificar Urgências (WhatsApp)</label>
                        </div>
                        <input type="text" placeholder="Anotar urgência do dia aqui..." class="mt-2 w-full bg-white border border-gray-300 rounded-md px-3 py-2 text-sm focus:ring-blue-500 focus:border-blue-500">
                    </li>

                    <!-- Prazos -->
                    <li>
                        <div class="task-item">
                            <input type="checkbox" id="p_prazos_check">
                            <label for="p_prazos_check" class="font-semibold">Analisar Prazos (Vencidos e Vincendos)</label>
                        </div>
                        <ul class="mt-3 ml-10 space-y-2 text-sm text-gray-600">
                            <li class="task-item"><input type="checkbox" id="p_p_minha_caixa"><label for="p_p_minha_caixa">Minha Caixa</label></li>
                            <li class="task-item"><input type="checkbox" id="p_p_everaldo"><label for="p_p_everaldo">Everaldo Júnior</label></li>
                            <li class="task-item"><input type="checkbox" id="p_p_izabelle"><label for="p_p_izabelle">Izabelle Dantas</label></li>
                            <li class="task-item"><input type="checkbox" id="p_p_jose"><label for="p_p_jose">José Leonardo (Promotor)</label></li>
                        </ul>
                    </li>

                    <!-- Prazos Judiciais -->
                    <li class="task-item">
                        <input type="checkbox" id="p_judicial_check">
                        <label for="p_judicial_check" class="font-semibold">Analisar Prazos Judiciais (resolver 1 dia antes)</label>
                    </li>
                    
                    <!-- Sem Movimento -->
                    <li class="task-item">
                        <input type="checkbox" id="p_movimento_check">
                        <label for="p_movimento_check" class="font-semibold">Verificar procedimentos sem movimento (+30 dias)</label>
                    </li>

                    <!-- Tempo extra -->
                    <li class="task-item">
                        <input type="checkbox" id="p_extra_check">
                        <label for="p_extra_check" class="font-semibold text-green-700">Se sobrar tempo: adiantar próximos vencimentos</label>
                    </li>
                </ul>
            </div>
        </main>

        <footer class="text-center mt-8">
            <button id="resetButton" class="bg-red-500 hover:bg-red-600 text-white font-bold py-2 px-6 rounded-lg transition-colors duration-300">
                Reiniciar para o Próximo Dia
            </button>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const resetButton = document.getElementById('resetButton');
            
            resetButton.addEventListener('click', () => {
                // Desmarca todos os checkboxes
                const checkboxes = document.querySelectorAll('input[type="checkbox"]');
                checkboxes.forEach(checkbox => {
                    checkbox.checked = false;
                });

                // Limpa todos os campos de texto
                const textInputs = document.querySelectorAll('input[type="text"]');
                textInputs.forEach(input => {
                    input.value = '';
                });

                // Rola para o topo da página
                window.scrollTo({ top: 0, behavior: 'smooth' });
            });
        });
    </script>
</body>
</html>
